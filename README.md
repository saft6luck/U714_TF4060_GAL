# U714_TF4060_GAL
This GAL is a fix for TF4060 CPU cards to allow Zorro 3 DMA to the extended 128MB RAM on these boards.
This is e.g. usefull for the A4091 SCSI board.

The GAL is inteded for use in all Amiga 3000(T) and 4000(T) and changes U714/P702 to remove the overlapping Zorro 3 space $10000000-$17FFFFFF from FAT BUSTER Z3 space.
This way FAT BUSTER will treat access to this Z3 space as mainboard access and allows Z3 cards to do DMA to this memory area.

Whith this fix, no other SW solutions are needed, like setting a Transfermask or use related tools.
