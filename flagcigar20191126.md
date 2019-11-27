1.Explain BAM FLAG value： 143?
143=128+8+4+2+1,即read paired,read mapped in pair,read unmapped,mate unmapped,second in pair.
该read是成对的paired reads中的一个，paired read中每个都正确比对到参考序列上，该read没有对比到参考序列上，该read成对的matepair read没有对比到参考序列上，在paired reads中，该read是与参考序列对比的第二条。
2.Explain BAM FLAG value： 99?
99=64+32+2+1,即read paired,read mapped in proper pair,mate reverse strand,first in pair.
该read是成对的paired reads中的一个，paired read中每个都正确比对到参考序列上，该read成对的matepair read其反向互补序列能够比对到参考序列，在paired reads中，该read是与参考序列对比的第一条。
3.Explain BAM FLAG value： 516?
516=512+4,即read unmapped,read fails platform/vendor quality checks.
该read没对比到参考序列上，该read没有通过质量控制。
4.Explain BAM FLAG value： 2064?
2064=2048+16，即read reverse strand,supplementary alignment.
该read其反向互补序列能够对比到参考序列，补充匹配的read。
5.Explain BAM FLAG value： 147?
147=128+16+2+1,即read paired,read mapped in proper pair,read reverse strand,second in pair.
该read是成对的paired reads中的一个，paired reads中每个都能正确对比到参考数列上，该read其反向互补序列能够对比到参考序列，在paired reads中，该read是与参考序列比对的第二条。 
6. Explain BAM CIGAR：14M2D31M
这条序列与参考基因相比，14bp碱基可以match，2bp碱基的删除，最后有31bp碱基的match。
7.Explain BAM CIGAR：3S6M1D5M
这条序列与参考基因相比，3bp的软裁剪（soft clipping），6bp的match，1bp的删除，5bp的match。
8.Explain BAM CIGAR: 6M14N5M
这条序列与参考序列相比，6bp的match，14bp的可变剪接位置，5bp的match。
9.Explain BAM CIGAR: 7M5D8M2I14M  (小写：7m5d8m2i14m）
这条序列与参考序列相比，7bp的match，5bp的碱基删除，8bp的match，2bp的碱基插入，14bp的match。
10. how long is the read with alignment CIGAR of 7M5D8M2I14M?
7+8+2+14=31bp
