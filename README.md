# pdf2change
PDF TOC editor for pdftk

## Installation
### Debian
`sudo apt install pdftk`

The idea come from this 2 videos

[![pdftk: Embedding a Table of Contents in a PDF file with pdftk][img1]][vid1]
[![Fix the page numbers in a PDF by using pdftk and inserting Page Labels][img2]][vid2]


## Video1: Insert TOC
```bash
# export data
pdftk input.pdf dump_data > metadata.txt

# import metadata
pdftk input.pdf update_info_utf8 edited_metadata.txt out output-w-TOC.pdf

```

## Video2: Edit PageNums

```bash
#uncompress file
pdftk input.pdf output-raw.pdf uncompress

#recompress
pdftk input-raw.pdf output-compr.pdf compress
```

## Example
Let me introduce you the best book that I read about the LinuxComand. 




<!-- Bibliografy -->
[img1]: https://img.youtube.com/vi/5dv_02v0zzc/0.jpg
[vid1]: https://www.youtube.com/watch?v=5dv_02v0zzc
[img2]: https://img.youtube.com/vi/zoH1Z_hSpak/0.jpg
[vid2]: https://www.youtube.com/watch?v=zoH1Z_hSpak
[webshell]: http://linuxcommand.org/index.php
[shellbook]: http://sourceforge.net/projects/linuxcommand/files/TLCL/19.01/TLCL-19.01.pdf/download
