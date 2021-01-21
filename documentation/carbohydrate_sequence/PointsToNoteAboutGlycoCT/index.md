# Points to note about GlycoCT

1. <a href="#1-underdetermined-capping-unit">Underdetermined capping unit</a>
2. <a href="#2-selection-of-residues-connecting-ambiguous-antenna-residues">Selection of residues connecting ambiguous antenna residues</a>
3. <a href="#3-change-of-substituent-type">Change of substituent type</a>
4. <a href="#4-available-substituents-in-glycoct">Available substituents in GlycoCT</a>


## 1. Underdetermined capping unit

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



## 2. Selection of residues connecting ambiguous antenna residues
1. Build glycan with a bracket using GlycoWorkbench (or GlycanBuilder)
![bracket1](https://user-images.githubusercontent.com/2530360/105280525-52d50100-5bed-11eb-9c0a-f6f10e2ee299.PNG)
1. Export to GlycoCT format
![bracket2](https://user-images.githubusercontent.com/2530360/105280578-6aac8500-5bed-11eb-83dc-878fc7abd261.PNG)
1. Find residues related to ambiguous antenna and their ID numbers in the GlycoCT
![bracket3 1](https://user-images.githubusercontent.com/2530360/105280605-78faa100-5bed-11eb-9023-f5860b93d7e2.png)
1. Change the ID numbers specified at "ParentIDs" in the GlycoCT to select parent residues of ambiguous antenna
    * Also need to change the connecting type in "SubtreeLinkageID"
![bracket4-1 1](https://user-images.githubusercontent.com/2530360/105280630-86b02680-5bed-11eb-9bff-b4d059e618db.png)
![bracket4-2 1](https://user-images.githubusercontent.com/2530360/105280653-97f93300-5bed-11eb-9cdb-b441b8362ce7.png)


## 3. Change of substituent type
1. Build glycan with a substituent using GlycoWorkbench (or GlycanBuilder)
    * The substituent must be able to convert to GlycoCT (e.g. phosphate)
![modSubstituent1](https://user-images.githubusercontent.com/2530360/105280991-72b8f480-5bee-11eb-88a7-a6c69cc13b81.PNG)
1. Export to GlycoCT format
![modSubstituent2](https://user-images.githubusercontent.com/2530360/105281025-88c6b500-5bee-11eb-8ab7-0eded070d139.PNG)
1. Find the substituent residue in the GlycoCT
1. Change the substituent name to the other one which you want to add
![modSubstituent4-1 1](https://user-images.githubusercontent.com/2530360/105281063-9ed47580-5bee-11eb-9192-247965ffaf1e.PNG)
![modSubstituent4-2 1](https://user-images.githubusercontent.com/2530360/105281079-a98f0a80-5bee-11eb-99cd-d25bfa55b445.PNG)


## 4. Available substituents in GlycoCT
![substituents](https://user-images.githubusercontent.com/2530360/105281469-99c3f600-5bef-11eb-8334-8168823e4cff.png)

 [Available substituents in GlycoCT](https://github.com/glycoinfo/GLIC/blob/master/documentation/carbohydrate_sequence/AvailableSubstituentsGlycoCT.md)
