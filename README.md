# redstaros_3.0_japanese(この方法では動作しません)

## stage2.imgを展開
```bash
cramfsswap stage2.img stage2_new.img
sudo fsck.cramfs --extract=fs stage2_new.img
```
この中の/usr/share/locale/に言語ファイルがあるので置き換える
## 圧縮
```bash
sudo mkfs.cramfs fs stage2_new.img
```
##iso作成
anyburnでisoの/redstar/base/stage2.imgを置き換える
修正版isolinux.cfgを入れる
lang=jaになっているほかvirtualboxで起動できるように編集、ログが見れるようにもしてある。

↑このようにやったが日本語にならない。誰か助けて。
