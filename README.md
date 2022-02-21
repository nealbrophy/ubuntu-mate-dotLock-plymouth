# Ubuntu Mate dotLock Plymouth Theme
This is a slightly customized version of [vikrashraghavan's dotLock](https://github.com/vikashraghavan/dotLock) (all I've done is whack the Ubuntu Mate logo into the center at the end of the animation).

## How to install
Assuming you're on Ubuntu Mate (otherwise why would you want to install this):
1. Clone this repo somewhere handy (e.g. your *Downloads* folder):
`git clone https://github.com/nealbrophy/ubuntu-mate-dotLock-plymouth`

2. Change directory into the cloned repo:
`cd ubuntu-mate-dotLock-plymouth`

3. Copy the inner *dotLockMate* folder to `/usr/share/plymouth/themes/` (__needs sudo priveleges__):
`sudo cp -r dotLockMate /usr/share/plymouth/themes/`

4. Install the theme:
`sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/dotLockMate/dotLockMate.plymouth 100`

5. Enable the theme (run the below then enter the number beside the theme you want to enable):
`sudo update-alternatives --config default.plymouth`
	- Enter the number that appears beside the theme you want to enable

6. Update boot:
`sudo update-initramfs -u`

