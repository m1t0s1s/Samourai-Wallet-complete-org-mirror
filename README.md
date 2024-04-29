# Samourai-Wallet-complete-org-mirror
Samourai Wallet complete org mirror


If you're trying to mirror samourai, they are on keybase.

https://keybase.io/samourai

The canary from archive.org's last fetch on april 24th does verify, ( the canary itself was updated on march 24th). https://web.archive.org/web/20240424023612/https://samouraiwallet.com/canary




Mirror the Samourai wallet source code

In powershell:

run:

gh auth login

Login with a browser with your account to get a token (prevents git spam imho). Your github account does _not_ need to be a member of the Samourai-Wallet github Org.

then run:

gh repo list Samourai-Wallet --json=nameWithOwner --limit 1000 -q ".[].nameWithOwner"  | %{gh repo clon
e $_}

size (476,939,295 bytes)
