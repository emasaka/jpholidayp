# jpholidayp

Is it holiday today in Japan?

## SYNOPSIS

    jpholidayp

## DESCRIPTION

Check "Is it holiday today?" in Japan.

No arguments, and no output.
Reports as exit status:

* 0 (success): holiday
* 1: not holiday

"Holiday" means:

* Sunday and Saturday
* In [holiday_jp](https://github.com/holiday-jp/holiday_jp)

It creates cache file at ~/.jpholidayp directory.

## EXAMPLES

usages in crontab.

    jpholidayp && some-command

Run some-command in holiday.

    jpholidayp || some-command

Run some-command in weekday.

## REQUIRES

* Python
* PyYAML

## PROXY

This program accesses internet server once in 5 days.

If you have to use proxy to access internet, set `https_proxy`
environment variable.

## AUTHOR

emasaka
