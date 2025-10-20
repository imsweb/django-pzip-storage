## 1.3.0 (in development)

* Drop support for Python 3.9
* Test on Python 3.14 and Django 5.2
* Support opening files for writing
* Allow `nocompress` option to accept a callable, or `True` to indicate never compress
* Experimental `rotate_storage` Django command for rotating file fields stored in `PZipStorage`


## 1.2.1 (2024-11-08)

*Note we skipped a version to align with `pzip`. Also, 1.2.0 was yanked due to incorrect
packaging.*

* Drop support for Django 3.x and Python 3.8
* Test on Django 5.x and Python 3.13
* Fixed an issue where the `needs_rotation` signal could be sent multiple times, and for
  invalid keys
* Require `pzip>=1.2.0` to address an issue on Python 3.13
* Expanded `PZipStorage.DEFAULT_NOCOMPRESS` to include more already-compressed filetypes
