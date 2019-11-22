# Points to note about GlycoCT

## Underdetermined capping unit

 * GlycoCT with the following glycan structure is using "u(-1+1)u" in GlycanBuilder. However, in the GlycoCT manual, as the type of identifier in the LIN section "u" is not described. Fig. 25 (p. 27) illustrates how to include an undetermined capping location. The notation used for the SubTreeLinkage is  "o(4+1)d". The linkage for the glycan structure [G02402FF](https://glytoucan.org/Structures/Glycans/G02402FF) shown below should be represented as "o(-1+1)d".
 
![GlyTouCan - G02402FF](https://image.glycosmos.org/snfg/png/G02402FF)

### incorrect GlycoCT 
#### Point: SubtreeLinkageID1:u(-1+1)u
```
RES
1b:b-dglc-HEX-1:5
2s:n-acetyl
3b:b-dglc-HEX-1:5
4s:n-acetyl
5b:b-dman-HEX-1:5
6b:a-dman-HEX-1:5
7b:a-dman-HEX-1:5
LIN
1:1d(2+1)2n
2:1o(4+1)3d
3:3d(2+1)4n
4:3o(4+1)5d
5:5o(3+1)6d
6:5o(6+1)7d
UND
UND1:100.0:100.0
ParentIDs:1|3|5|6|7
SubtreeLinkageID1:u(-1+1)u
RES
8b:x-dman-HEX-1:5
```

### correct GlycoCT
#### Point: SubtreeLinkageID1:o(-1+1)d
```
RES
1b:b-dglc-HEX-1:5
2s:n-acetyl
3b:b-dglc-HEX-1:5
4s:n-acetyl
5b:b-dman-HEX-1:5
6b:a-dman-HEX-1:5
7b:a-dman-HEX-1:5
LIN
1:1d(2+1)2n
2:1o(4+1)3d
3:3d(2+1)4n
4:3o(4+1)5d
5:5o(3+1)6d
6:5o(6+1)7d
UND
UND1:100.0:100.0
ParentIDs:1|3|5|6|7
SubtreeLinkageID1:o(-1+1)d
RES
8b:x-dman-HEX-1:5
```

