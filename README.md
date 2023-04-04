# HW3 Aksenov Yaroslav
[Ссылка на ноутбук](https://colab.research.google.com/drive/1FkXcUdyfBThQeP0zhH5uCWZ6PT77YLtZ?usp=sharing)

## Взятые гистоновые метки
Название | Название файла
--- | ---
H3K79me2 | wgEncodeBroadHistoneA549H3k79me2Dex100nmAlnRep1.bam
H3K9me3 | wgEncodeBroadHistoneA549H3k09me3Etoh02AlnRep1.bam
H3K36me3 | wgEncodeBroadHistoneA549H3k36me3Dex100nmAlnRep1.bam
H3K27me3 | wgEncodeBroadHistoneA549H3k27me3Dex100nmAlnRep1.bam
H3K4me2 | wgEncodeBroadHistoneA549H3k04me2Dex100nmAlnRep1.bam
H3K9ac | wgEncodeBroadHistoneA549H3k09acEtoh02AlnRep1.bam
H3K4me3 | wgEncodeBroadHistoneA549H3k04me3Dex100nmAlnRep1.bam
H3K4me1 | wgEncodeBroadHistoneA549H3k04me1Dex100nmAlnRep1.bam
H3K27ac | wgEncodeBroadHistoneA549H3k27acDex100nmAlnRep1.bam
H4K20me1 | wgEncodeBroadHistoneA549H4k20me1Etoh02AlnRep1.bam

## [Файл cellmarkfiletable.txt](data/cellmarkfiletable.txt)
## Картинки из ChromHMM

![Image](/data/emissions_15.png)
![Image](/data/A549_15_overlap.png)
![Image](/data/transitions_15.png)

![Image](/data/A549_15_RefSeqTSS_neighborhood.png)
![Image](/data/A549_15_RefSeqTES_neighborhood.png)

## Эпигенетические типы
№ | Название | Описание | Картинка
 --- | --- | ---| ---
1 | Active Promoter | <ul><li> H3K27me3, H3K4me2, H3K4me3 </li><li> на интрон или экзон </li> | ![Image](/data/type_1.png)
2 | Weak enhancer/Weak transcribed | <ul><li> H3K4me1, H3K4me2 </li><li> Находятся на RefSeqTES, RefSeqGene, а также на ядерной ламине </li><li> на интрон </li> | ![Image](/data/type_2.png)
3 | Strong enhancer/Transcriptional elogation | <ul><li> H3K9ac, H3K27ac, H3K4me1, H3K4me2, H3K4me3 </li><li> Находятся на RefSeqTES и RefSeqTSS2Kb, а также на ядерной ламине </li><li> на интрон </li> | ![Image](/data/type_3.png)
4 | Active Promoter | <ul><li> H3K9ac, H3K27ac, H3K4me3, H3K4me2 </li><li>  Находятся на CpGIslands, RefSeqTES, RefSeqExon и RefSeqTSS2Kb </li><li> на интрон или экзон </li> | ![Image](/data/type_4.png)
5 | Active Promoter | <ul><li> H3K9ac, H3K27ac, H3K4me3, H3K4me2 </li><li>  Находятся на RefSeqTES и RefSeqTSS2Kb, а также на RefSeqExon, CpGIslands, и RefSeqGene </li><li> на интрон или экзон </li> | ![Image](/data/type_5.png)
6 | Weak enhancer | <ul><li>  H3K79me2, H3K9ac, H3K27ac, H3K4me3, H3K4me2 </li><li>  Находятся на RefSeqGene и RefSeqTES, а также RefSeqExon, но реже </li><li> на интрон </li> | ![Image](/data/type_6.png)
7 | Weak enhancer | <ul><li>  H3K9ac, H3K27ac, H3K4me1 </li><li>  Находятся на RefSeqTES </li><li> на интрон </li> | ![Image](/data/type_7.png)
8 | Weak enhancer | <ul><li>  H3K4me1 </li><li>  Находятся на RefSeqTES, а также на ядерной ламине, но реже </li><li> на интрон </li> | ![Image](/data/type_8.png)
9 | Weak enhancer | <ul><li>  H3K79me2, H3K4me1 </li><li>  Находятся на RefSeqGene, а также RefSeqTES и RefSeqExon, но реже </li><li> на интрон </li> | ![Image](/data/type_9.png)
10 | Weak transcribed | <ul><li>  H3K79me2 </li><li>  Находятся на RefSeqGene </li><li> на экзон или интрон </li> | ![Image](/data/type_10.png)
11 | Weak transcribed | <ul><li>  H3K36me3, H3K79me2 </li><li>  Находятся на RefSeqGene, а также на RefSeqTES и RefSeqExon, но реже </li><li> на экзон или интрон </li> | ![Image](/data/type_11.png)
12 | Weak transcribed | <ul><li>  H3K36me3 </li><li>  Находятся на RefSeqGene, а также на RefSeqTES и RefSeqExon, но реже </li><li> на экзон или интрон </li> | ![Image](/data/type_12.png)
13 | Repressed | <ul><li>  Находятся на ядерной ламине, то есть на участок репрессированного гетерохроматима </li><li> Не попадает никуда </li> | ![Image](/data/type_13.png)
14 | Heterochromatin | <ul><li>  H3K27me3 </li><li>  Находятся на ядерной ламине, то есть на участок репрессированного гетерохроматима </li><li> Не попадает никуда </li> | ![Image](/data/type_14.png)
15 | Heterochromatin | <ul><li>  H3K9me3 </li><li>  Находятся на ядерной ламине, то есть на участок репрессированного гетерохроматима </li><li> Не попадает никуда </li> | ![Image](/data/type_15.png)
 
## [Результат бонусного задания .bed файл](data/new_A549_15_dense.bed)