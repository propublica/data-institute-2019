# Open Refine Troubleshooting for Macs

If your computer tells you that Open Refine is damaged, follow these steps and try again:

1. Open System Preferences
2. Open Security & Privacy
3. Go to the General Tab
4. Change the "Allow applications downloaded from:" setting to "Anywhere"
5. Try opening Open Refine again.

If you don't see the "Anywhere" option, do the following:
1. Open up the [Termainal App](https://en.wikipedia.org/wiki/Terminal_(OS_X))
2. Copy and paste this exact command into it: `sudo spctl --master-disable`
3. Push enter. It should ask you for your computer's password.
4. Enter your password, and know that the cursor won't move, but the computer is listening.
5. Once you're done, your settings should be automatically changed to "Anywhere."
6. Try opening Open Refine again.

