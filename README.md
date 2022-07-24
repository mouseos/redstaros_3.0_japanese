# redstaros_3.0_japanese

##stage2.imgを展開

cramfsswap stage2.img stage2_new.img
sudo fsck.cramfs --extract=fs stage2_new.img
