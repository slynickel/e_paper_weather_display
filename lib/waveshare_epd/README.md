These are the files copied out of https://github.com/waveshare/e-Paper

Few notes:
* There is no license file I could find in that repo. There's just the embedded license clause in each file header.
* The `sysfs*.so` files are old, last commit on them 04d4621789dd6832222e1c7be8f04f93f51df33 Fri Dec 11 14:36:30 2020 +0800. They are needed.
  They appear to be compiled through the make file but haven't changed much I guess? I looked through them with a few debug tools doesn't appear to be anything malicious 
  though you should generally be wary of running junk you find on the internet.
* If you're using a different size E-Paper display you'll need to swap in the correct version. This is direct linking the files that work for the 7x5in display I had.
* I think all raspberry PIs are ARM64 architecture. If not you're going to have problems as the *.so files are ARM architecture.

