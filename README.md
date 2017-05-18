# Quick and Dirty data to Mifare 1K V0.1.0

Simply takes a file (<= 720 bytes) and writes it to a mifare 1k file using the ER301 interface.

Makes use of Marc de Verdelhan's 2013 code for YHY523U under MIT license.

My contributions also under MIT.

### Usage

Make sure you have the file to be written called datafile in the same directory as er301_backup

```
$ ./er301_backup
```

To verify run

```
$ diff -s datafile outfile
```


### Changelog

* 2017/05/18 - Initial commit

### Todo

* Add meta data to first sector 32 bytes.