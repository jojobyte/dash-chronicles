### Wants
https://discord.com/channels/745481679786868746/1078448819332726835

#### \@coolaj86
- Contacts (QR, Name, Email)
- Cash Drawer (denoms of coin, # of mixes)
   - 2 x Đ10 @ 10 exchanges
   - 2 x Đ1 @ 10 exchanges
   - 5 x Đ0.5 @ 10 exchanges
- Subscription (approve contact for ĐX/month)
- Categorizing Expenses and report
   - (lifetime, this month, today)
- Track daily avg price with expense
   - (and spot price?)
- Tracking where a coin in connected to other coins in the wallet
- https://trello.com/c/6XAuy9DW/94-request-new-concept#comment-6400ed856fe149503e8fc021
	- Functional Requirements
		1. User & Productivity-focused (e.g. like Venmo or Mint)
		2. Browser-friendly, and Fast (i.e. using the new Dash Tools SDK) 
	- Features
		- social: share xpub QRs with contacts via SMS, email, etc (like Venmo)
		-  convenient: access multiple accounts, categorize expenses, savings goals
		-  smart: use crowdnode for interest-earning savings accounts
		-  commercial: subscription payments, MEGA-like pre-payment links (key-in-hash, pubs-on-service)
		-  small: doesn't rely on local blockchain sync for account balances
		-  fast: using our Dash Tools SDK with modern JS libraries that loads instantly
		-  decentralized: the user can select insight and live wallet APIs that they trust
		-  secure: denominated cash-drawer payments to protect privacy
		-  integrated: can work with other apps and services like DashDirect, without fingerprinting change
		-  modern: using secp256k1, DashPhrase, DashKeys, DashHD, DashTx, and DashSight
		-  desktop: using Tauri or similar to provide OS integration for file storage, possibly send SMS or email via the OS default app
- Priorities:
	- share with contacts
	- cash drawer with denominated coins
	- work with DashDirect on browser mobile
- Connect Options
	- Share or Request Contact
	- Request Subscription or single Payment
	- Send Payment Key
	- Send Wallet Key (e.g. for shared / linked accounts between people or devices)
- Scan
	- Subscription (XPub, Payment Protocol)
	- Contact (XPub)
	- Shared Account (XPrv)
	- Request for Payment (Address, Payment Protocol)
	- One-Time Payment (WIF)
- Spreadsheet / Table Copying
	- HTML Tables when copied become something like a CSV file that can be pasted into spreadsheet software (excel or google sheets) maintaining their column & row structure
- Each contact should be a side-by-side view:
	- The half of the contact that you've received from them, and the half of the contact that you would send them.
	- Repeating the context: You, as a user, don't have an XPub / QR that represents you. There is a different XPub for each half of each relationship. ^XPubPairing
	- The XPub is generated when you want to request money from the other person. You send them the thing that they send the money to.
	- We can create links or QRs that are XPubs or have information for requesting an XPub, but those links or QRs will be pairwise, not singleton.

#### \@jojobyte
- Invest and earn interest like a savings account
	- CrowdNode
- dark mode
- Dash to Gift Card
	- DashDirect is US only
	- Bitrefill might be decent alternative or additional integration
		- Used by Edge Wallet..?
- This Wallet would be some mix of:
	- manage some amount of your Dash holdings
	- view transactions
	- generate new addresses
	- invest through something like crowdnode
	- spend like cash through something like Dash Direct or Bitrefill
	- send dash to friends/contacts via alias similar to venmo usernames
- With an undertone of
	- Prove the `dash-tools` 
		- Are a useful alternative to Dash Core Lib (which is a fork of Bitcoin Lib & are massive in file size)
		- work by using them in all the scenarios a Wallet would need
	- Pay people with Dash but by username.
- All that said, the target should be anyone, maybe slightly tech savvy, but if you can use Venmo I think you should be able to use this.

#### \@rion
- DashDirect (gift card & prepaid Visa card purchases with Dash).
- THORChain/Maya (yield on savings for liquidity provision, cross crypto swaps).
- CrowdNode (yield on savings, like @jojobyte mentioned)
- other integrations
- a web wallet 
- a desktop wrapper using Tauri.
- locally named contacts and friending using AJ's strategy
- https://trello.com/c/6XAuy9DW/94-request-new-concept#comment-6401072d97c288be118633c0
	- start with a "reference wallet application" approach - same as we did with CrowdNode - where we use our modern [Dash Tools](https://github.com/dashhive/dash-tools) to scaffold a vanilla HTML/CSS/JS web app that anyone can use as a reference for building modern, performant Dash wallets with key features.
- What this wallet is supposed to showcase (from my perspective) is:
	1.  That our wallet tools work
	2.  That we can create a username/contact-oriented onboarding experience that's pleasant and easy.
	3.  That we can send and receive payments to/from contacts.
- **All I want right now is a flow where two people can make a connection (friend request) and then pay each other.**