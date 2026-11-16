# Westpac Online Banking — Hackathon Prototype

A concept prototype for the "AI and what it means for Banking" hackathon.

A self-contained single-page mock of a Westpac-style online banking site featuring multi-user demo profiles, transaction creation, savings plans, BankSmart AI budgeting, and persistence.

- Styled with GEL-inspired design tokens (Westpac red `#DA1710`).
- Features BankSmart AI settings for income splitting (into pots) and transaction round-up increments ($1, $5, $10, $50, $100).
- Bills bucket lists the recurring bills BankSmart has detected.
- `index.html` is fully self-contained — just open it in any modern browser.

---

## Pre-populated Demo Profiles

On the login screen, click the **👤 Demo accounts ▾** button in the bottom-left corner to quickly switch between demo users, or type any of their 8-digit Customer IDs directly into the login form:

| Customer ID | Name | Role | Profile & Accounts |
| :--- | :--- | :--- | :--- |
| `21157077` | **Alex Chen** *(Default)* | Young renter | Saving for a rental bond. Accounts: *Westpac Choice*, *Westpac Life* (Rental bond goal), *Low Rate Card*, and *COMPANY PTY LTD* business banking. |
| `18524718` | **Priya Sharma** | Family budgeter | Managing household finances. Accounts: *Westpac Choice*, *Westpac Life* (Family holiday & Kids' education goals), *Altitude Black Card*. Personal only. |
| `90815760` | **Sam Rossi** | Café owner | Director of Rollers Pty Ltd. Accounts: Personal *Choice* & *Life*, *Business Platinum Card*, and *Westpac Business One* with merchant settlement. Defaults to Business view. |
| `13138554` | **Margaret "Peggy" Wilson** | Retiree (age 71) | Living on Age Pension + super income. Accounts: *Westpac Choice*, *Westpac Life* (Grandkids' Christmas, Caravan trip, Rates bucket), and *Westpac Term Deposit* ($40,000 at 4.60% p.a.). |

*Entering any other credentials will default to signing in as Alex Chen.*

---

## Adding Transactions

On any account's transaction screen, click the **💳 + Add transaction** button in the bottom-left corner:
1. Select **Debit (− money out)** or **Credit (+ money in)**.
2. Choose the destination account (automatically pre-selects the account you are viewing).
3. Type a description or pick from convenient presets (e.g. ☕ Coffee, 🛒 Groceries, 💼 Salary).
4. Enter an amount and date.
5. Review the real-time balance preview and click **Add Transaction**.
6. The transaction is instantly recorded, running balances are recalculated, and personal everyday spending updates your **Safe to spend** allowance in BankSmart.

---

## Data Persistence & Reset

All demo data is automatically persisted in browser storage:
- **`localStorage` (`wbc_demo_v1`)**: Stores all accounts, custom transactions, saving goals/buckets, and Wesley AI preferences per user.
- **`sessionStorage` (`wbc_demo_user`)**: Maintains your active session across page reloads.
- **Resetting Data**: Click **👤 Demo accounts ▾** on the login screen and choose **↺ Reset all demo data** at any time to restore initial seed balances and transactions.

---

**Not affiliated with or endorsed by Westpac. Demonstration only.**
