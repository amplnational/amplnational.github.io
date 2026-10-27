# Chapter Portal setup

The portal (`portal.html`) uses **Firebase**, a free Google service, for logins and data. You only need to do this setup once, and it takes about 15 minutes.

## 1. Create the Firebase project
1. Go to <https://console.firebase.google.com> and sign in with the AMPL National Google account.
2. Click **Create a project**, name it `ampl-portal`, and turn off Google Analytics. Click **Create**.

## 2. Turn on email/password login
1. In the left menu: **Build → Authentication → Get started**.
2. Under **Sign-in method**, click **Email/Password**, enable the first toggle, and click **Save**.
3. Open the **Settings** tab, then **Authorized domains**, then **Add domain**. Add `amplnational.com`.

## 3. Create the database
1. In the left menu: **Build → Firestore Database → Create database**.
2. Choose a location (`us-west2` is closest to California) and start in **production mode**.
3. Open the **Rules** tab. Delete everything there, paste in the full contents of `firestore.rules` from this repo, and click **Publish**.

## 4. Connect the website
1. Click the gear icon, then **Project settings**. Under **Your apps**, click the **`</>`** (Web) icon.
2. Name it `ampl-website`. Leave Hosting unchecked. Click **Register app**.
3. Firebase shows a `firebaseConfig = { ... }` block. Copy each value into the matching line of `firebase-config.js` in this repo.
4. Commit and push.

These values are meant to be public. The security rules are what protect your data.

## 5. Make yourself the first admin
1. Go to `https://amplnational.com/portal.html`, click **Request Access**, and sign up.
2. In the Firebase console: **Firestore Database → Data → users →** click your account's document.
3. Change the `role` field from `pending` to `admin`.
4. Refresh the portal. You'll see the admin tabs.
5. Go to **Chapters & Budgets** and click the button to add the existing chapters.

## Day-to-day use
- **New chapter officers** go to the portal and click **Request Access**. They then show up under **Approvals** and **Accounts**. Assign them a chapter, set the role to **Chapter officer**, and click **Save**.
- **Additional National board members:** set their role to **National admin**.
- **Budgets:** set each chapter's base allocation under **Chapters & Budgets**. Chapters request grants through **Finances**, and you approve or deny each request under **Approvals**.
- **Reimbursements:** after an event, an officer opens **Reimbursements** and fills in the grant, the event, the total spent, who to pay back with their Zelle or Venmo, and photos of the receipts. If they spent more than the grant, they have to explain why. You'll see it under **Reimbursements → To pay** (and as a count next to **Approvals**). Send the money, check the amount, and click **Mark as paid**, or **Deny** with a reason. Marking paid adds the payment to the **National Ledger**. **Undo** puts a request back in the queue (and removes its ledger entry) if you clicked by mistake.
- **National Ledger:** National's own books, replacing the "Budget & Finance Tracker" sheet: fundraising, income, banquet expenses and national expenses, with the remaining balance. **Download for Google Sheets** gives you a copy to open in Sheets.

## Updating the security rules
Whenever `firestore.rules` changes in this repo, paste the whole file into **Firestore Database → Rules** again (replacing everything) and click **Publish**. The reimbursements and ledger features need the version that includes `reimbursements`, `receipts` and `ledger`.

## Importing the old budget sheet (one time)
`ledger-import.csv` in the repo folder holds the rows from "AMPL National — Budget & Finance Tracker v2". It is excluded from git so the finances never become public. In the portal, open **National Ledger → Import from CSV** and choose that file. The import button only appears while the ledger is empty, so it can't be imported twice.

Receipts are stored in Firestore (Firebase Storage requires the paid plan). Photos are shrunk in the browser; PDFs must be under 700 KB.
- **Removing someone:** click **Remove** in **Accounts**. To delete their login entirely, also go to Firebase console → **Authentication** → **Users**.

## What each role can do
| | Pending | Chapter officer | National admin |
|---|---|---|---|
| Read announcements & resources | — | ✓ | ✓ (and post) |
| Edit chapter profile | — | own chapter | all |
| Submit event reports | — | own chapter | view all |
| Budget requests | — | submit / withdraw own | approve / deny |
| Reimbursements | — | submit / withdraw own | mark paid / deny |
| National Ledger | — | — | ✓ |
| Ledger (expenses & income) | — | own chapter | all |
| Set budget allocations | — | — | ✓ |
| Approve accounts | — | — | ✓ |

## Testing in Codespaces
The portal works on `localhost` without extra setup. If you open it through a Codespaces forwarded address (`*.app.github.dev`), add that domain under **Authentication → Settings → Authorized domains** first.
