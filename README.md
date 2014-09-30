# MailMate Customizations

## Mailbox Layouts

The files [correspondence arc.plist](Layouts/Mailboxes/correspondence arc.plist) and [correspondence arc (widescreen).plist](Layouts/Mailboxes/correspondence arc (widescreen)) combine the *Correspondence* view with the *Thread Arcs* view. **Correspondence Arc** is designed more for a taller, more narrow, view, while **Correspondence Arc (Widescreen)** is designed for more for a widescreen layout. Additionally, in **Correspondence Arc** I hide the Messages sidebar and either use the Gmail shortcuts or ⌘T to access the *Go to Mailbox* feature.

![Correspondence Arc, with hidden sidebar](delete-me/correspondence-arc.png)

![Correspondence Arc (Widescreen)](delete-me/correspondence-arc-widescreen.png)

## Keybindings

| File | Description |
| :--- | :--- | :--- |
| `composer.plist` | Shortcuts for the email composition window |
| `gmail.plist` | Gmail style shortcuts in the main viewer window |
| `trackpad-gestures.plist` | Trackpad gestures as outlined in the manual |

These are fairly self-explanatory if you look through the `plist` files. They should be placed in

	~/Library/Application Support/MailMate/Resources/KeyBindings

NOTE: You may need to make the KeyBindings folder if you don't already have one. See [installation](#installation) below.

#### Some comments about `gmail.plist`

The keybindings in this file are, for the most part, identical to those included in MailMate. I have, however, included a couple of (IMHO) improvements:

| Shortcut | Description
| :---:    | :---
| j/k      | move between all messages (instead of threads)
| n/p      | move between mailboxes (which I find more useful)
| gg       | move to the top of the list (Vim-style)
| ⇧G       | move to the bottom (Vim-style)
| /        | search all messages
| u        | go to the inbox
| #        | delete the current message
| ⌘⇧F      | forward message as an attachment
| ⇧E       | archive all messages in the current thread
| ⌘↩       | send message

## Installation

Mailmate user customizations are stored in `~/Library/Application Support/MailMate/Resources`. If you don't have any customizations, I'll suggest doing this:

	mkdir -p "$HOME/Library/Application Support/MailMate/Resources"
	git clone https://github.com/chauncey-garrett/mailmate.git "$HOME/Library/Application Support/MailMate/Resources"

## Like it?

Add it to your toolbox; if not, open an [issue!](https://github.com/chauncey-garrett/mailmate/issues "chauncey-garrett/mailmate/issues") I appreciate all feedback.

## Author(s)

I specifically want to thank [Benny Kjær Nielsen](http://freron.com/about/index.html#about_me) for making this repository possible by producing [MailMate](http://freron.com), and for providing excellent customer support for when I have had questions about how to best make these customizations.

*The author(s) of this module should be contacted via the [issue tracker](https://github.com/chauncey-garrett/mailmate/issues "chauncey-garrett/mailmate/issues").*

  - [Chauncey Garrett](https://github.com/chauncey-garrett "chauncey-garrett")
