# How to use GlycanBuilder2 software

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

