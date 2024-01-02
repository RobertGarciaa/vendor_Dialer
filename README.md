## Add In Rom

Add This Line In device.mk

$(call inherit-product, vendor/Dialer/Dialer.mk)

And you will need to remove the following text from the directory root similar to the one below.
LOCAL_OVERRIDES_PACKAGES := Dialer

You need to remove the following folders using the local manifest:
/packages/apps/dialer

# AOSP Dialer From Crdroid
If you use this dialer as the default dialer, you can see the call recording function work and the incoming call number be displayed properly when using VOLTE.(https://github.com/search?q=Disable+redir_party_num&type=commits)

## Credits

Thanks to [Chaitanyakm](https://github.com/Chaitanyakm/vendor_bcr) For Base Repo And [Crdroid](https://github.com/crdroidandroid) For Base Source
