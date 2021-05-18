# How to use GlycanBuilder2 software

## Download GlycanBuilder2

* https://github.com/glycoinfo/Executable/blob/master/GlycanBuilder2/GlycanBuilder2_for_mac.zip
  * GlycanBuilder2_for_mac.zip

* Unzip the zip file
* Double-click "run.command" in the unzipped folder.
  * If you do not have java installed, please install it.


## How to draw a high mannose glycan

* Video https://www.youtube.com/watch?v=yY1al648RvI


[![](https://img.youtube.com/vi/yY1al648RvI/0.jpg)](https://www.youtube.com/watch?v=yY1al648RvI)


* Add linkage information if necessary.

## Correction of GlycoCT: Underdetermined capping unit

* [Points to note about GlycoCT](https://glic.glycoinfo.org/documentation/carbohydrate_sequence/PointsToNoteAboutGlycoCT/)
  * SubtreeLinkageID1:u(-1+1)u --> SubtreeLinkageID1:o(-1+1)d

```
RES
1b:b-dglc-HEX-1:5
2s:n-acetyl
3b:b-dglc-HEX-1:5
4s:n-acetyl
5b:b-dman-HEX-1:5
6b:a-dman-HEX-1:5
7b:a-dman-HEX-1:5
8b:a-dman-HEX-1:5
9b:a-dman-HEX-1:5
10b:a-dman-HEX-1:5
LIN
1:1d(2+1)2n
2:1o(4+1)3d
3:3d(2+1)4n
4:3o(4+1)5d
5:5o(3+1)6d
6:6o(2+1)7d
7:5o(6+1)8d
8:8o(3+1)9d
9:8o(6+1)10d
UND
UND1:100.0:100.0
ParentIDs:1|3|5|6|7|8|9|10
SubtreeLinkageID1:u(-1+1)u  ---> SubtreeLinkageID1:o(-1+1)d
RES
11b:x-dman-HEX-1:5
UND2:100.0:100.0
ParentIDs:1|3|5|6|7|8|9|10
SubtreeLinkageID1:u(-1+1)u  ---> SubtreeLinkageID1:o(-1+1)d
RES
12b:x-dman-HEX-1:5
UND3:100.0:100.0
ParentIDs:1|3|5|6|7|8|9|10
SubtreeLinkageID1:u(-1+1)u  ---> SubtreeLinkageID1:o(-1+1)d
RES
13b:x-dman-HEX-1:5
UND4:100.0:100.0
ParentIDs:1|3|5|6|7|8|9|10
SubtreeLinkageID1:u(-1+1)u  ---> SubtreeLinkageID1:o(-1+1)d
RES
14b:x-dman-HEX-1:5
UND5:100.0:100.0
ParentIDs:1|3|5|6|7|8|9|10
SubtreeLinkageID1:u(-1+1)u  ---> SubtreeLinkageID1:o(-1+1)d
RES
15b:x-dman-HEX-1:5
UND6:100.0:100.0
ParentIDs:1|3|5|6|7|8|9|10
SubtreeLinkageID1:u(-1+1)u  ---> SubtreeLinkageID1:o(-1+1)d
RES
16b:x-dman-HEX-1:5
UND7:100.0:100.0
ParentIDs:1|3|5|6|7|8|9|10
SubtreeLinkageID1:u(-1+1)u  ---> SubtreeLinkageID1:o(-1+1)d
RES
17b:x-dman-HEX-1:5
UND8:100.0:100.0
ParentIDs:1|3|5|6|7|8|9|10
SubtreeLinkageID1:u(-1+1)u  ---> SubtreeLinkageID1:o(-1+1)d
RES
18b:x-dman-HEX-1:5
UND9:100.0:100.0
ParentIDs:1|3|5|6|7|8|9|10
SubtreeLinkageID1:u(-1+1)u  ---> SubtreeLinkageID1:o(-1+1)d
RES
19b:x-dman-HEX-1:5
UND10:100.0:100.0
ParentIDs:1|3|5|6|7|8|9|10
SubtreeLinkageID1:u(-1+1)u  ---> SubtreeLinkageID1:o(-1+1)d
RES
20b:x-dman-HEX-1:5
```


## Correct GlycoCT format

```
RES
1b:b-dglc-HEX-1:5
2s:n-acetyl
3b:b-dglc-HEX-1:5
4s:n-acetyl
5b:b-dman-HEX-1:5
6b:a-dman-HEX-1:5
7b:a-dman-HEX-1:5
8b:a-dman-HEX-1:5
9b:a-dman-HEX-1:5
10b:a-dman-HEX-1:5
LIN
1:1d(2+1)2n
2:1o(4+1)3d
3:3d(2+1)4n
4:3o(4+1)5d
5:5o(3+1)6d
6:6o(2+1)7d
7:5o(6+1)8d
8:8o(3+1)9d
9:8o(6+1)10d
UND
UND1:100.0:100.0
ParentIDs:1|3|5|6|7|8|9|10
SubtreeLinkageID1:o(-1+1)d
RES
11b:x-dman-HEX-1:5
UND2:100.0:100.0
ParentIDs:1|3|5|6|7|8|9|10
SubtreeLinkageID1:o(-1+1)d
RES
12b:x-dman-HEX-1:5
UND3:100.0:100.0
ParentIDs:1|3|5|6|7|8|9|10
SubtreeLinkageID1:o(-1+1)d
RES
13b:x-dman-HEX-1:5
UND4:100.0:100.0
ParentIDs:1|3|5|6|7|8|9|10
SubtreeLinkageID1:o(-1+1)d
RES
14b:x-dman-HEX-1:5
UND5:100.0:100.0
ParentIDs:1|3|5|6|7|8|9|10
SubtreeLinkageID1:o(-1+1)d
RES
15b:x-dman-HEX-1:5
UND6:100.0:100.0
ParentIDs:1|3|5|6|7|8|9|10
SubtreeLinkageID1:o(-1+1)d
RES
16b:x-dman-HEX-1:5
UND7:100.0:100.0
ParentIDs:1|3|5|6|7|8|9|10
SubtreeLinkageID1:o(-1+1)d
RES
17b:x-dman-HEX-1:5
UND8:100.0:100.0
ParentIDs:1|3|5|6|7|8|9|10
SubtreeLinkageID1:o(-1+1)d
RES
18b:x-dman-HEX-1:5
UND9:100.0:100.0
ParentIDs:1|3|5|6|7|8|9|10
SubtreeLinkageID1:o(-1+1)d
RES
19b:x-dman-HEX-1:5
UND10:100.0:100.0
ParentIDs:1|3|5|6|7|8|9|10
SubtreeLinkageID1:o(-1+1)d
RES
20b:x-dman-HEX-1:5
```

## Confirmation of glycan structure

* Move to GlycoNAVI GlycanFormatConverter site (https://glyconavi.org/Tools/tool/gfc.php).
* Paste the modified GlycoCT into the input box below the GlycoCT to WURCS. (Please delete the GlycoCT you have already entered.) 

![image](https://user-images.githubusercontent.com/2530360/118645479-f3dd6c80-b819-11eb-9116-5d21170a383d.png)

* You can get the result of conversion from GlycoCT format to WURCS format.

![image](https://user-images.githubusercontent.com/2530360/118644871-3783a680-b819-11eb-84e8-a74cec5813ca.png)

* Copies the converted WURCS string.

![image](https://user-images.githubusercontent.com/2530360/118644989-53874800-b819-11eb-9903-52eb94c5f2a7.png)


* Move to GlycoNAVI GlyCosmos API site (https://glyconavi.org/Tools/tool/cosmos.php).

* Paste the WURCS into the input box below the Glycan Images. (Please delete the WURCS you have already entered.)
* 
![GlycoNAVI-GFC](https://user-images.githubusercontent.com/2530360/118644344-ad3b4280-b818-11eb-8ca0-f3c49e494391.png)

* Click the Convert button.

* The following glycan structures can be confirmed.

![image](https://user-images.githubusercontent.com/2530360/118645271-ac56e080-b819-11eb-9003-5defb786932c.png)





