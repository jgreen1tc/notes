Main memory is organized into 4k (4096 byte) pages. As programs use more memory than is available in main memory, the operating system finds pages that havent been used in awhile and writes their conents to the Page Dataset(s), freeing that page of main memory for use by another program. When a program references a page that isn't in memory, a "page fault" is generated 

Segment, page, and regeion tables keep track of storage

Frame - 4k piece of real storage
Slot - 4k record in a page data set
MVS storage managers keep track of pages, frames, and slots
