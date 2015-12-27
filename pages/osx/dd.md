# dd

> convert and copy a file

- Make a bootable usb drive from a iso file

`dd if={{file.iso}} of=/dev/{{usb drive}}`

- clone a drive to another drive with 4MB block and ignore error

`dd if=/dev/{{source drive}} of=/dev/{{dest drive}} bs=4m conv=noerror`

- Wipe a disk by writing random data to it

`dd if=/dev/urandom of=/dev/{{dest drive}}`

- Benchmarking drive write performance

`dd if=/dev/zero of={{file_1GB}} bs=1024 count=1000000`
