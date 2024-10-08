# Bug Bounty program

## Introduction
Ok listen, we all hate bugs. That's why we have this program to reward you for hunting bugs for us.

## Details
Bugs will be categorized as follows:
| Level      | Impact    |
| ---------- | ---------------- |
| `Low`      | - Changing details of other users (including modifying browser local storage) without already-connected wallet interaction and with significant user interaction, such as:<br>- Iframing leading to modifying the backend/browser state (must demonstrate impact with PoC)    <br>- Taking over broken or expired outgoing links, such as:  <br>- Social media handles, etc.  <br>- Temporarily disabling user to access target site, such as:  <br>- Locking up the victim from login. <br>- Cookie bombing, etc.|
| `Medium`   | - Changing non-sensitive details of other users (including modifying browser local storage) without already-connected wallet interaction and with up to one click of user interaction, such as:<br>- Changing the first/last name of user<br>- Enabling/disabling notifications<br>- Injecting/modifying the static content on the target application without JavaScript (reflected), such as:<br>- Reflected HTML injection<br>- Loading external site data<br>- Redirecting users to malicious websites (open redirect)|
| `High`     | - Injecting/modifying the static content on the target application without JavaScript (persistent), such as:<br>- HTML injection without JavaScript<br>- Replacing existing text with arbitrary text<br>- Arbitrary file uploads, etc.<br>- Changing sensitive details of other users (including modifying browser local storage) without already-connected wallet interaction and with up to one click of user interaction, such as:<br>- Email or password of the victim, etc.<br>- Improperly disclosing confidential user information, such as:<br>- Email address<br>- Phone number<br>- Physical address, etc.<br>- Subdomain takeover without already-connected wallet interaction|
| `Critical` | - Execute arbitrary system commands<br>- Retrieve sensitive data/files from a running server, such as:<br>  - /etc/shadow<br>  - database passwords<br>  - blockchain keys<br>(this does not include non-sensitive environment variables, open source code, or usernames)<br>- Taking down the application/website<br>- Taking down the NFT URI<br>- Taking state-modifying authenticated actions (with or without blockchain state interaction) on behalf of other users without any interaction by that user, such as:<br>  - Changing registration information<br>  - Commenting<br>  - Voting<br>  - Making trades<br>  - Withdrawals, etc.<br>- Changing the NFT metadata<br>- Subdomain takeover with already-connected wallet interaction<br>- Direct theft of user funds<br>- Malicious interactions with an already-connected wallet, such as:<br>  - Modifying transaction arguments or parameters<br>  - Substituting contract addresses<br>  - Submitting malicious transactions<br>- Direct theft of user NFTs<br>- Injection of malicious HTML or XSS through NFT metadata |

## Submission guidelines
Please submit information to the following email `dev@kaia.io` with the email subject 
```
SECURITY: [insert bug title]
```