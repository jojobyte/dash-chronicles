### Path 1
1. User visits website
	1. For the first time
		- User is prompted to either:
			1. generate new wallet & setup desired @alias
				- Eg. @jojobyte
			2. provide recovery phrase to restore existing wallet & set desired @alias
		- *See https://dashhive.github.io/crowdnode-ui/#!/wallet for example*
	2. With a wallet setup, User should see:
		1. Dash Balance
		2. Add Contact Button
			- Opens Add Contact Modal
				- Input Xpub field with Scan QR Code button
				- Optional Name Field (local reference)
			- User connects with new contact via Xpub and saves with @alias
				- @jojobyte shares Xpub (QR Code or dash protocol link) with @coolaj86
					- `dash://<address>?<amount,etc>`
					- `dash:XpubJojobyteExampleNotReal?mutual=true` *not real*
					- `dash:xpub6EeJWM8tq4B8LVB1K6MBxD37yaVqJOJOvHV4m9Ahty4GBq9khPfiUTdhgeucJrVq54Ydtq74vywfBYTEncnefkzfRvGwB2zU2A8GACSUAxN?mutual=true` *also not real*
				- @coolaj86 scans QR or pastes dash protocol link in field and adds @jojobyte's Xpub as contact
					- if `mutual=true` is appended to dash protocol link, automate @jojobyte adding @coolaj86
				- @coolaj86 shares Xpub with @jojobyte
				- @jojobyte adds @coolaj86's Xpub as contact
		3. Receive/Deposit/Request Funds Button
			- Opens QR Modal
				- Toggle between normal Dash Address or @alias xpub system
		4. Send/Withdraw Funds Button
			- Opens Sending Modal
				- Dash Amount
				- Input field for Dash address, @alias with select from contacts button
				- *Send Ð2.00 to @coolaj86*
		5. Manage Contacts
			- A list displaying contacts with per-contact controls to Send/Request funds, edit & remove
				- MVP only able to edit name

### Path 2
- TODO