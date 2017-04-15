# api documentation for  [moment-timezone (v0.5.13)](http://momentjs.com/timezone/)  [![npm package](https://img.shields.io/npm/v/npmdoc-moment-timezone.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-moment-timezone) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-moment-timezone.svg)](https://travis-ci.org/npmdoc/node-npmdoc-moment-timezone)
#### Parse and display moments in any timezone.

[![NPM](https://nodei.co/npm/moment-timezone.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/moment-timezone)

[![apidoc](https://npmdoc.github.io/node-npmdoc-moment-timezone/build/screenCapture.buildCi.browser.apidoc.html.png)](https://npmdoc.github.io/node-npmdoc-moment-timezone/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-moment-timezone/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-moment-timezone/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Tim Wood",
        "url": "http://timwoodcreates.com/"
    },
    "bugs": {
        "url": "https://github.com/moment/moment-timezone/issues"
    },
    "dependencies": {
        "moment": ">= 2.9.0"
    },
    "description": "Parse and display moments in any timezone.",
    "devDependencies": {
        "grunt": "0.4.5",
        "grunt-contrib-clean": "0.6.0",
        "grunt-contrib-jshint": "0.11.2",
        "grunt-contrib-nodeunit": "0.4.1",
        "grunt-contrib-uglify": "0.9.1"
    },
    "directories": {},
    "dist": {
        "shasum": "99ce5c7d827262eb0f1f702044177f60745d7b90",
        "tarball": "https://registry.npmjs.org/moment-timezone/-/moment-timezone-0.5.13.tgz"
    },
    "engines": {
        "node": "*"
    },
    "gitHead": "2b8da8f103f019949d45dc86fd6763960c8474d8",
    "homepage": "http://momentjs.com/timezone/",
    "jspm": {
        "main": "builds/moment-timezone-with-data",
        "shim": {
            "moment-timezone": {
                "deps": [
                    "moment"
                ]
            }
        }
    },
    "keywords": [
        "moment",
        "date",
        "time",
        "timezone",
        "olson",
        "iana",
        "zone",
        "tz"
    ],
    "license": "MIT",
    "main": "./index.js",
    "maintainers": [
        {
            "name": "ichernev"
        },
        {
            "name": "maggiepint"
        },
        {
            "name": "mj1856"
        },
        {
            "name": "timrwood"
        }
    ],
    "name": "moment-timezone",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/moment/moment-timezone.git"
    },
    "scripts": {
        "test": "grunt"
    },
    "version": "0.5.13"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module moment-timezone](#apidoc.module.moment-timezone)
1.  boolean <span class="apidocSignatureSpan">moment-timezone.</span>suppressDeprecationWarnings
1.  [function <span class="apidocSignatureSpan"></span>moment-timezone ()](#apidoc.element.moment-timezone.moment-timezone)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>ISO_8601 ()](#apidoc.element.moment-timezone.ISO_8601)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>RFC_2822 ()](#apidoc.element.moment-timezone.RFC_2822)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>calendarFormat (myMoment, now)](#apidoc.element.moment-timezone.calendarFormat)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>createFromInputFallback ()](#apidoc.element.moment-timezone.createFromInputFallback)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>defineLocale (name, config)](#apidoc.element.moment-timezone.defineLocale)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>duration (input, key)](#apidoc.element.moment-timezone.duration)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>invalid (flags)](#apidoc.element.moment-timezone.invalid)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>isDate (input)](#apidoc.element.moment-timezone.isDate)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>isDuration (obj)](#apidoc.element.moment-timezone.isDuration)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>isMoment (obj)](#apidoc.element.moment-timezone.isMoment)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>lang ()](#apidoc.element.moment-timezone.lang)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>langData ()](#apidoc.element.moment-timezone.langData)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>locale (key, values)](#apidoc.element.moment-timezone.locale)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>localeData (key)](#apidoc.element.moment-timezone.localeData)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>locales ()](#apidoc.element.moment-timezone.locales)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>max ()](#apidoc.element.moment-timezone.max)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>min ()](#apidoc.element.moment-timezone.min)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>months (format, index)](#apidoc.element.moment-timezone.months)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>monthsShort (format, index)](#apidoc.element.moment-timezone.monthsShort)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>normalizeUnits (units)](#apidoc.element.moment-timezone.normalizeUnits)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>now ()](#apidoc.element.moment-timezone.now)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>parseTwoDigitYear (input)](#apidoc.element.moment-timezone.parseTwoDigitYear)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>parseZone ()](#apidoc.element.moment-timezone.parseZone)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>relativeTimeRounding (roundingFunction)](#apidoc.element.moment-timezone.relativeTimeRounding)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>relativeTimeThreshold (threshold, limit)](#apidoc.element.moment-timezone.relativeTimeThreshold)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>toString ()](#apidoc.element.moment-timezone.toString)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>tz (input)](#apidoc.element.moment-timezone.tz)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>tz.Zone (packedString)](#apidoc.element.moment-timezone.tz.Zone)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>unix (input)](#apidoc.element.moment-timezone.unix)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>updateLocale (name, config)](#apidoc.element.moment-timezone.updateLocale)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>updateOffset (mom, keepTime)](#apidoc.element.moment-timezone.updateOffset)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>utc (input, format, locale, strict)](#apidoc.element.moment-timezone.utc)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>weekdays (localeSorted, format, index)](#apidoc.element.moment-timezone.weekdays)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>weekdaysMin (localeSorted, format, index)](#apidoc.element.moment-timezone.weekdaysMin)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>weekdaysShort (localeSorted, format, index)](#apidoc.element.moment-timezone.weekdaysShort)
1.  object <span class="apidocSignatureSpan">moment-timezone.</span>defaultZone
1.  object <span class="apidocSignatureSpan">moment-timezone.</span>deprecationHandler
1.  object <span class="apidocSignatureSpan">moment-timezone.</span>duration.fn
1.  object <span class="apidocSignatureSpan">moment-timezone.</span>fn
1.  object <span class="apidocSignatureSpan">moment-timezone.</span>momentProperties
1.  object <span class="apidocSignatureSpan">moment-timezone.</span>tz.Zone.prototype
1.  string <span class="apidocSignatureSpan">moment-timezone.</span>defaultFormat
1.  string <span class="apidocSignatureSpan">moment-timezone.</span>defaultFormatUtc
1.  string <span class="apidocSignatureSpan">moment-timezone.</span>version

#### [module moment-timezone.duration](#apidoc.module.moment-timezone.duration)
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>duration (input, key)](#apidoc.element.moment-timezone.duration.duration)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.</span>invalid ()](#apidoc.element.moment-timezone.duration.invalid)
1.  object <span class="apidocSignatureSpan">moment-timezone.duration.</span>fn

#### [module moment-timezone.duration.fn](#apidoc.module.moment-timezone.duration.fn)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>_bubble ()](#apidoc.element.moment-timezone.duration.fn._bubble)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>abs ()](#apidoc.element.moment-timezone.duration.fn.abs)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>add (input, value)](#apidoc.element.moment-timezone.duration.fn.add)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>as (units)](#apidoc.element.moment-timezone.duration.fn.as)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>asDays ()](#apidoc.element.moment-timezone.duration.fn.asDays)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>asHours ()](#apidoc.element.moment-timezone.duration.fn.asHours)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>asMilliseconds ()](#apidoc.element.moment-timezone.duration.fn.asMilliseconds)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>asMinutes ()](#apidoc.element.moment-timezone.duration.fn.asMinutes)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>asMonths ()](#apidoc.element.moment-timezone.duration.fn.asMonths)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>asSeconds ()](#apidoc.element.moment-timezone.duration.fn.asSeconds)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>asWeeks ()](#apidoc.element.moment-timezone.duration.fn.asWeeks)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>asYears ()](#apidoc.element.moment-timezone.duration.fn.asYears)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>days ()](#apidoc.element.moment-timezone.duration.fn.days)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>get (units)](#apidoc.element.moment-timezone.duration.fn.get)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>hours ()](#apidoc.element.moment-timezone.duration.fn.hours)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>humanize (withSuffix)](#apidoc.element.moment-timezone.duration.fn.humanize)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>isValid ()](#apidoc.element.moment-timezone.duration.fn.isValid)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>lang ()](#apidoc.element.moment-timezone.duration.fn.lang)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>locale (key)](#apidoc.element.moment-timezone.duration.fn.locale)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>localeData ()](#apidoc.element.moment-timezone.duration.fn.localeData)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>milliseconds ()](#apidoc.element.moment-timezone.duration.fn.milliseconds)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>minutes ()](#apidoc.element.moment-timezone.duration.fn.minutes)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>months ()](#apidoc.element.moment-timezone.duration.fn.months)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>seconds ()](#apidoc.element.moment-timezone.duration.fn.seconds)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>subtract (input, value)](#apidoc.element.moment-timezone.duration.fn.subtract)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>toISOString ()](#apidoc.element.moment-timezone.duration.fn.toISOString)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>toIsoString ()](#apidoc.element.moment-timezone.duration.fn.toIsoString)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>toJSON ()](#apidoc.element.moment-timezone.duration.fn.toJSON)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>toString ()](#apidoc.element.moment-timezone.duration.fn.toString)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>valueOf ()](#apidoc.element.moment-timezone.duration.fn.valueOf)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>weeks ()](#apidoc.element.moment-timezone.duration.fn.weeks)
1.  [function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>years ()](#apidoc.element.moment-timezone.duration.fn.years)

#### [module moment-timezone.fn](#apidoc.module.moment-timezone.fn)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>add (val, period)](#apidoc.element.moment-timezone.fn.add)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>calendar (time, formats)](#apidoc.element.moment-timezone.fn.calendar)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>clone ()](#apidoc.element.moment-timezone.fn.clone)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>creationData ()](#apidoc.element.moment-timezone.fn.creationData)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>date (value)](#apidoc.element.moment-timezone.fn.date)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>dates ()](#apidoc.element.moment-timezone.fn.dates)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>day (input)](#apidoc.element.moment-timezone.fn.day)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>dayOfYear (input)](#apidoc.element.moment-timezone.fn.dayOfYear)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>days (input)](#apidoc.element.moment-timezone.fn.days)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>daysInMonth ()](#apidoc.element.moment-timezone.fn.daysInMonth)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>diff (input, units, asFloat)](#apidoc.element.moment-timezone.fn.diff)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>endOf (units)](#apidoc.element.moment-timezone.fn.endOf)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>format (inputString)](#apidoc.element.moment-timezone.fn.format)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>from (time, withoutSuffix)](#apidoc.element.moment-timezone.fn.from)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>fromNow (withoutSuffix)](#apidoc.element.moment-timezone.fn.fromNow)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>get (units)](#apidoc.element.moment-timezone.fn.get)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>hasAlignedHourOffset (input)](#apidoc.element.moment-timezone.fn.hasAlignedHourOffset)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>hour (value)](#apidoc.element.moment-timezone.fn.hour)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>hours (value)](#apidoc.element.moment-timezone.fn.hours)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>inspect ()](#apidoc.element.moment-timezone.fn.inspect)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>invalidAt ()](#apidoc.element.moment-timezone.fn.invalidAt)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isAfter (input, units)](#apidoc.element.moment-timezone.fn.isAfter)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isBefore (input, units)](#apidoc.element.moment-timezone.fn.isBefore)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isBetween (from, to, units, inclusivity)](#apidoc.element.moment-timezone.fn.isBetween)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isDST ()](#apidoc.element.moment-timezone.fn.isDST)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isDSTShifted ()](#apidoc.element.moment-timezone.fn.isDSTShifted)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isLeapYear ()](#apidoc.element.moment-timezone.fn.isLeapYear)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isLocal ()](#apidoc.element.moment-timezone.fn.isLocal)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isSame (input, units)](#apidoc.element.moment-timezone.fn.isSame)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isSameOrAfter (input, units)](#apidoc.element.moment-timezone.fn.isSameOrAfter)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isSameOrBefore (input, units)](#apidoc.element.moment-timezone.fn.isSameOrBefore)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isUTC ()](#apidoc.element.moment-timezone.fn.isUTC)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isUtc ()](#apidoc.element.moment-timezone.fn.isUtc)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isUtcOffset ()](#apidoc.element.moment-timezone.fn.isUtcOffset)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isValid ()](#apidoc.element.moment-timezone.fn.isValid)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isoWeek (input)](#apidoc.element.moment-timezone.fn.isoWeek)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isoWeekYear (input)](#apidoc.element.moment-timezone.fn.isoWeekYear)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isoWeekday (input)](#apidoc.element.moment-timezone.fn.isoWeekday)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isoWeeks (input)](#apidoc.element.moment-timezone.fn.isoWeeks)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isoWeeksInYear ()](#apidoc.element.moment-timezone.fn.isoWeeksInYear)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>lang ()](#apidoc.element.moment-timezone.fn.lang)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>local (keepLocalTime)](#apidoc.element.moment-timezone.fn.local)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>locale (key)](#apidoc.element.moment-timezone.fn.locale)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>localeData ()](#apidoc.element.moment-timezone.fn.localeData)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>max ()](#apidoc.element.moment-timezone.fn.max)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>millisecond (value)](#apidoc.element.moment-timezone.fn.millisecond)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>milliseconds (value)](#apidoc.element.moment-timezone.fn.milliseconds)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>min ()](#apidoc.element.moment-timezone.fn.min)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>minute (value)](#apidoc.element.moment-timezone.fn.minute)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>minutes (value)](#apidoc.element.moment-timezone.fn.minutes)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>month (value)](#apidoc.element.moment-timezone.fn.month)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>months ()](#apidoc.element.moment-timezone.fn.months)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>parseZone ()](#apidoc.element.moment-timezone.fn.parseZone)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>parsingFlags ()](#apidoc.element.moment-timezone.fn.parsingFlags)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>quarter (input)](#apidoc.element.moment-timezone.fn.quarter)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>quarters (input)](#apidoc.element.moment-timezone.fn.quarters)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>second (value)](#apidoc.element.moment-timezone.fn.second)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>seconds (value)](#apidoc.element.moment-timezone.fn.seconds)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>set (units, value)](#apidoc.element.moment-timezone.fn.set)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>startOf (units)](#apidoc.element.moment-timezone.fn.startOf)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>subtract (val, period)](#apidoc.element.moment-timezone.fn.subtract)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>to (time, withoutSuffix)](#apidoc.element.moment-timezone.fn.to)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>toArray ()](#apidoc.element.moment-timezone.fn.toArray)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>toDate ()](#apidoc.element.moment-timezone.fn.toDate)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>toISOString ()](#apidoc.element.moment-timezone.fn.toISOString)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>toJSON ()](#apidoc.element.moment-timezone.fn.toJSON)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>toNow (withoutSuffix)](#apidoc.element.moment-timezone.fn.toNow)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>toObject ()](#apidoc.element.moment-timezone.fn.toObject)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>toString ()](#apidoc.element.moment-timezone.fn.toString)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>tz (name)](#apidoc.element.moment-timezone.fn.tz)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>unix ()](#apidoc.element.moment-timezone.fn.unix)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>utc ()](#apidoc.element.moment-timezone.fn.utc)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>utcOffset (input, keepLocalTime, keepMinutes)](#apidoc.element.moment-timezone.fn.utcOffset)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>valueOf ()](#apidoc.element.moment-timezone.fn.valueOf)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>week (input)](#apidoc.element.moment-timezone.fn.week)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>weekYear (input)](#apidoc.element.moment-timezone.fn.weekYear)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>weekday (input)](#apidoc.element.moment-timezone.fn.weekday)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>weeks (input)](#apidoc.element.moment-timezone.fn.weeks)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>weeksInYear ()](#apidoc.element.moment-timezone.fn.weeksInYear)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>year (value)](#apidoc.element.moment-timezone.fn.year)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>years ()](#apidoc.element.moment-timezone.fn.years)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>zone ()](#apidoc.element.moment-timezone.fn.zone)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>zoneAbbr ()](#apidoc.element.moment-timezone.fn.zoneAbbr)
1.  [function <span class="apidocSignatureSpan">moment-timezone.fn.</span>zoneName ()](#apidoc.element.moment-timezone.fn.zoneName)

#### [module moment-timezone.tz](#apidoc.module.moment-timezone.tz)
1.  boolean <span class="apidocSignatureSpan">moment-timezone.tz.</span>moveAmbiguousForward
1.  boolean <span class="apidocSignatureSpan">moment-timezone.tz.</span>moveInvalidForward
1.  [function <span class="apidocSignatureSpan">moment-timezone.</span>tz (input)](#apidoc.element.moment-timezone.tz.tz)
1.  [function <span class="apidocSignatureSpan">moment-timezone.tz.</span>Zone (packedString)](#apidoc.element.moment-timezone.tz.Zone)
1.  [function <span class="apidocSignatureSpan">moment-timezone.tz.</span>add (packed)](#apidoc.element.moment-timezone.tz.add)
1.  [function <span class="apidocSignatureSpan">moment-timezone.tz.</span>guess (ignoreCache)](#apidoc.element.moment-timezone.tz.guess)
1.  [function <span class="apidocSignatureSpan">moment-timezone.tz.</span>link (aliases)](#apidoc.element.moment-timezone.tz.link)
1.  [function <span class="apidocSignatureSpan">moment-timezone.tz.</span>load (data)](#apidoc.element.moment-timezone.tz.load)
1.  [function <span class="apidocSignatureSpan">moment-timezone.tz.</span>names ()](#apidoc.element.moment-timezone.tz.names)
1.  [function <span class="apidocSignatureSpan">moment-timezone.tz.</span>needsOffset (m)](#apidoc.element.moment-timezone.tz.needsOffset)
1.  [function <span class="apidocSignatureSpan">moment-timezone.tz.</span>setDefault (name)](#apidoc.element.moment-timezone.tz.setDefault)
1.  [function <span class="apidocSignatureSpan">moment-timezone.tz.</span>unpack (string)](#apidoc.element.moment-timezone.tz.unpack)
1.  [function <span class="apidocSignatureSpan">moment-timezone.tz.</span>unpackBase60 (string)](#apidoc.element.moment-timezone.tz.unpackBase60)
1.  [function <span class="apidocSignatureSpan">moment-timezone.tz.</span>zone (name, caller)](#apidoc.element.moment-timezone.tz.zone)
1.  [function <span class="apidocSignatureSpan">moment-timezone.tz.</span>zoneExists (name)](#apidoc.element.moment-timezone.tz.zoneExists)
1.  object <span class="apidocSignatureSpan">moment-timezone.tz.</span>_links
1.  object <span class="apidocSignatureSpan">moment-timezone.tz.</span>_names
1.  object <span class="apidocSignatureSpan">moment-timezone.tz.</span>_zones
1.  string <span class="apidocSignatureSpan">moment-timezone.tz.</span>dataVersion
1.  string <span class="apidocSignatureSpan">moment-timezone.tz.</span>version

#### [module moment-timezone.tz.Zone](#apidoc.module.moment-timezone.tz.Zone)
1.  [function <span class="apidocSignatureSpan">moment-timezone.tz.</span>Zone (packedString)](#apidoc.element.moment-timezone.tz.Zone.Zone)

#### [module moment-timezone.tz.Zone.prototype](#apidoc.module.moment-timezone.tz.Zone.prototype)
1.  [function <span class="apidocSignatureSpan">moment-timezone.tz.Zone.prototype.</span>_index (timestamp)](#apidoc.element.moment-timezone.tz.Zone.prototype._index)
1.  [function <span class="apidocSignatureSpan">moment-timezone.tz.Zone.prototype.</span>_set (unpacked)](#apidoc.element.moment-timezone.tz.Zone.prototype._set)
1.  [function <span class="apidocSignatureSpan">moment-timezone.tz.Zone.prototype.</span>abbr (mom)](#apidoc.element.moment-timezone.tz.Zone.prototype.abbr)
1.  [function <span class="apidocSignatureSpan">moment-timezone.tz.Zone.prototype.</span>offset (mom)](#apidoc.element.moment-timezone.tz.Zone.prototype.offset)
1.  [function <span class="apidocSignatureSpan">moment-timezone.tz.Zone.prototype.</span>parse (timestamp)](#apidoc.element.moment-timezone.tz.Zone.prototype.parse)



# <a name="apidoc.module.moment-timezone"></a>[module moment-timezone](#apidoc.module.moment-timezone)

#### <a name="apidoc.element.moment-timezone.moment-timezone"></a>[function <span class="apidocSignatureSpan"></span>moment-timezone ()](#apidoc.element.moment-timezone.moment-timezone)
- description and source-code
```javascript
function hooks() {
    return hookCallback.apply(null, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.ISO_8601"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>ISO_8601 ()](#apidoc.element.moment-timezone.ISO_8601)
- description and source-code
```javascript
ISO_8601 = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.RFC_2822"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>RFC_2822 ()](#apidoc.element.moment-timezone.RFC_2822)
- description and source-code
```javascript
RFC_2822 = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.calendarFormat"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>calendarFormat (myMoment, now)](#apidoc.element.moment-timezone.calendarFormat)
- description and source-code
```javascript
function getCalendarFormat(myMoment, now) {
    var diff = myMoment.diff(now, 'days', true);
    return diff < -6 ? 'sameElse' :
            diff < -1 ? 'lastWeek' :
            diff < 0 ? 'lastDay' :
            diff < 1 ? 'sameDay' :
            diff < 2 ? 'nextDay' :
            diff < 7 ? 'nextWeek' : 'sameElse';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.createFromInputFallback"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>createFromInputFallback ()](#apidoc.element.moment-timezone.createFromInputFallback)
- description and source-code
```javascript
createFromInputFallback = function () {
    if (hooks.deprecationHandler != null) {
        hooks.deprecationHandler(null, msg);
    }
    if (firstTime) {
        var args = [];
        var arg;
        for (var i = 0; i < arguments.length; i++) {
            arg = '';
            if (typeof arguments[i] === 'object') {
                arg += '\n[' + i + '] ';
                for (var key in arguments[0]) {
                    arg += key + ': ' + arguments[0][key] + ', ';
                }
                arg = arg.slice(0, -2); // Remove trailing comma and space
            } else {
                arg = arguments[i];
            }
            args.push(arg);
        }
        warn(msg + '\nArguments: ' + Array.prototype.slice.call(args).join('') + '\n' + (new Error()).stack);
        firstTime = false;
    }
    return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.defineLocale"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>defineLocale (name, config)](#apidoc.element.moment-timezone.defineLocale)
- description and source-code
```javascript
function defineLocale(name, config) {
    if (config !== null) {
        var parentConfig = baseConfig;
        config.abbr = name;
        if (locales[name] != null) {
            deprecateSimple('defineLocaleOverride',
                    'use moment.updateLocale(localeName, config) to change ' +
                    'an existing locale. moment.defineLocale(localeName, ' +
                    'config) should only be used for creating a new locale ' +
                    'See http://momentjs.com/guides/#/warnings/define-locale/ for more info.');
            parentConfig = locales[name]._config;
        } else if (config.parentLocale != null) {
            if (locales[config.parentLocale] != null) {
                parentConfig = locales[config.parentLocale]._config;
            } else {
                if (!localeFamilies[config.parentLocale]) {
                    localeFamilies[config.parentLocale] = [];
                }
                localeFamilies[config.parentLocale].push({
                    name: name,
                    config: config
                });
                return null;
            }
        }
        locales[name] = new Locale(mergeConfigs(parentConfig, config));

        if (localeFamilies[name]) {
            localeFamilies[name].forEach(function (x) {
                defineLocale(x.name, x.config);
            });
        }

        // backwards compat for now: also set the locale
        // make sure we set the locale AFTER all child locales have been
        // created, so we won't end up with the child locale set.
        getSetGlobalLocale(name);


        return locales[name];
    } else {
        // useful for testing
        delete locales[name];
        return null;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>duration (input, key)](#apidoc.element.moment-timezone.duration)
- description and source-code
```javascript
function createDuration(input, key) {
    var duration = input,
        // matching against regexp is expensive, do it on demand
        match = null,
        sign,
        ret,
        diffRes;

    if (isDuration(input)) {
        duration = {
            ms : input._milliseconds,
            d  : input._days,
            M  : input._months
        };
    } else if (isNumber(input)) {
        duration = {};
        if (key) {
            duration[key] = input;
        } else {
            duration.milliseconds = input;
        }
    } else if (!!(match = aspNetRegex.exec(input))) {
        sign = (match[1] === '-') ? -1 : 1;
        duration = {
            y  : 0,
            d  : toInt(match[DATE])                         * sign,
            h  : toInt(match[HOUR])                         * sign,
            m  : toInt(match[MINUTE])                       * sign,
            s  : toInt(match[SECOND])                       * sign,
            ms : toInt(absRound(match[MILLISECOND] * 1000)) * sign // the millisecond decimal point is included in the match
        };
    } else if (!!(match = isoRegex.exec(input))) {
        sign = (match[1] === '-') ? -1 : 1;
        duration = {
            y : parseIso(match[2], sign),
            M : parseIso(match[3], sign),
            w : parseIso(match[4], sign),
            d : parseIso(match[5], sign),
            h : parseIso(match[6], sign),
            m : parseIso(match[7], sign),
            s : parseIso(match[8], sign)
        };
    } else if (duration == null) {// checks for null or undefined
        duration = {};
    } else if (typeof duration === 'object' && ('from' in duration || 'to' in duration)) {
        diffRes = momentsDifference(createLocal(duration.from), createLocal(duration.to));

        duration = {};
        duration.ms = diffRes.milliseconds;
        duration.M = diffRes.months;
    }

    ret = new Duration(duration);

    if (isDuration(input) && hasOwnProp(input, '_locale')) {
        ret._locale = input._locale;
    }

    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.invalid"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>invalid (flags)](#apidoc.element.moment-timezone.invalid)
- description and source-code
```javascript
function createInvalid(flags) {
    var m = createUTC(NaN);
    if (flags != null) {
        extend(getParsingFlags(m), flags);
    }
    else {
        getParsingFlags(m).userInvalidated = true;
    }

    return m;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.isDate"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>isDate (input)](#apidoc.element.moment-timezone.isDate)
- description and source-code
```javascript
function isDate(input) {
    return input instanceof Date || Object.prototype.toString.call(input) === '[object Date]';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.isDuration"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>isDuration (obj)](#apidoc.element.moment-timezone.isDuration)
- description and source-code
```javascript
function isDuration(obj) {
    return obj instanceof Duration;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.isMoment"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>isMoment (obj)](#apidoc.element.moment-timezone.isMoment)
- description and source-code
```javascript
function isMoment(obj) {
    return obj instanceof Moment || (obj != null && obj._isAMomentObject != null);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.lang"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>lang ()](#apidoc.element.moment-timezone.lang)
- description and source-code
```javascript
lang = function () {
    if (hooks.deprecationHandler != null) {
        hooks.deprecationHandler(null, msg);
    }
    if (firstTime) {
        var args = [];
        var arg;
        for (var i = 0; i < arguments.length; i++) {
            arg = '';
            if (typeof arguments[i] === 'object') {
                arg += '\n[' + i + '] ';
                for (var key in arguments[0]) {
                    arg += key + ': ' + arguments[0][key] + ', ';
                }
                arg = arg.slice(0, -2); // Remove trailing comma and space
            } else {
                arg = arguments[i];
            }
            args.push(arg);
        }
        warn(msg + '\nArguments: ' + Array.prototype.slice.call(args).join('') + '\n' + (new Error()).stack);
        firstTime = false;
    }
    return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.langData"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>langData ()](#apidoc.element.moment-timezone.langData)
- description and source-code
```javascript
langData = function () {
    if (hooks.deprecationHandler != null) {
        hooks.deprecationHandler(null, msg);
    }
    if (firstTime) {
        var args = [];
        var arg;
        for (var i = 0; i < arguments.length; i++) {
            arg = '';
            if (typeof arguments[i] === 'object') {
                arg += '\n[' + i + '] ';
                for (var key in arguments[0]) {
                    arg += key + ': ' + arguments[0][key] + ', ';
                }
                arg = arg.slice(0, -2); // Remove trailing comma and space
            } else {
                arg = arguments[i];
            }
            args.push(arg);
        }
        warn(msg + '\nArguments: ' + Array.prototype.slice.call(args).join('') + '\n' + (new Error()).stack);
        firstTime = false;
    }
    return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.locale"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>locale (key, values)](#apidoc.element.moment-timezone.locale)
- description and source-code
```javascript
function getSetGlobalLocale(key, values) {
    var data;
    if (key) {
        if (isUndefined(values)) {
            data = getLocale(key);
        }
        else {
            data = defineLocale(key, values);
        }

        if (data) {
            // moment.duration._locale = moment._locale = data;
            globalLocale = data;
        }
    }

    return globalLocale._abbr;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.localeData"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>localeData (key)](#apidoc.element.moment-timezone.localeData)
- description and source-code
```javascript
function getLocale(key) {
    var locale;

    if (key && key._locale && key._locale._abbr) {
        key = key._locale._abbr;
    }

    if (!key) {
        return globalLocale;
    }

    if (!isArray(key)) {
        //short-circuit everything else
        locale = loadLocale(key);
        if (locale) {
            return locale;
        }
        key = [key];
    }

    return chooseLocale(key);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.locales"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>locales ()](#apidoc.element.moment-timezone.locales)
- description and source-code
```javascript
function listLocales() {
    return keys$1(locales);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.max"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>max ()](#apidoc.element.moment-timezone.max)
- description and source-code
```javascript
function max() {
    var args = [].slice.call(arguments, 0);

    return pickBy('isAfter', args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.min"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>min ()](#apidoc.element.moment-timezone.min)
- description and source-code
```javascript
function min() {
    var args = [].slice.call(arguments, 0);

    return pickBy('isBefore', args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.months"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>months (format, index)](#apidoc.element.moment-timezone.months)
- description and source-code
```javascript
function listMonths(format, index) {
    return listMonthsImpl(format, index, 'months');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.monthsShort"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>monthsShort (format, index)](#apidoc.element.moment-timezone.monthsShort)
- description and source-code
```javascript
function listMonthsShort(format, index) {
    return listMonthsImpl(format, index, 'monthsShort');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.normalizeUnits"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>normalizeUnits (units)](#apidoc.element.moment-timezone.normalizeUnits)
- description and source-code
```javascript
function normalizeUnits(units) {
    return typeof units === 'string' ? aliases[units] || aliases[units.toLowerCase()] : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.now"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>now ()](#apidoc.element.moment-timezone.now)
- description and source-code
```javascript
now = function () {
    return Date.now ? Date.now() : +(new Date());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.parseTwoDigitYear"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>parseTwoDigitYear (input)](#apidoc.element.moment-timezone.parseTwoDigitYear)
- description and source-code
```javascript
parseTwoDigitYear = function (input) {
    return toInt(input) + (toInt(input) > 68 ? 1900 : 2000);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.parseZone"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>parseZone ()](#apidoc.element.moment-timezone.parseZone)
- description and source-code
```javascript
function createInZone() {
    return createLocal.apply(null, arguments).parseZone();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.relativeTimeRounding"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>relativeTimeRounding (roundingFunction)](#apidoc.element.moment-timezone.relativeTimeRounding)
- description and source-code
```javascript
function getSetRelativeTimeRounding(roundingFunction) {
    if (roundingFunction === undefined) {
        return round;
    }
    if (typeof(roundingFunction) === 'function') {
        round = roundingFunction;
        return true;
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.relativeTimeThreshold"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>relativeTimeThreshold (threshold, limit)](#apidoc.element.moment-timezone.relativeTimeThreshold)
- description and source-code
```javascript
function getSetRelativeTimeThreshold(threshold, limit) {
    if (thresholds[threshold] === undefined) {
        return false;
    }
    if (limit === undefined) {
        return thresholds[threshold];
    }
    thresholds[threshold] = limit;
    if (threshold === 's') {
        thresholds.ss = limit - 1;
    }
    return true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.toString"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>toString ()](#apidoc.element.moment-timezone.toString)
- description and source-code
```javascript
toString = function () {
    return toString;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.tz"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>tz (input)](#apidoc.element.moment-timezone.tz)
- description and source-code
```javascript
function tz(input) {
		var args = Array.prototype.slice.call(arguments, 0, -1),
			name = arguments[arguments.length - 1],
			zone = getZone(name),
			out  = moment.utc.apply(null, args);

		if (zone && !moment.isMoment(input) && needsOffset(out)) {
			out.add(zone.parse(out), 'minutes');
		}

		out.tz(name);

		return out;
	}
```
- example usage
```shell
...

[![NPM version][npm-version-image]][npm-url] [![NPM downloads][npm-downloads-image]][npm-url] [![MIT License][license-image]][license
-url] [![Build Status][travis-image]][travis-url]

IANA Time Zone Database + [Moment.js](http://momentjs.com).

'''js
var june = moment("2014-06-01T12:00:00Z");
june.tz('America/Los_Angeles').format('ha z'); // 5am PDT
june.tz('America/New_York').format('ha z');    // 8am EDT
june.tz('Asia/Tokyo').format('ha z');          // 9pm JST
june.tz('Australia/Sydney').format('ha z');    // 10pm EST

var dec = moment("2014-12-01T12:00:00Z");
dec.tz('America/Los_Angeles').format('ha z');  // 4am PST
dec.tz('America/New_York').format('ha z');     // 7am EST
...
```

#### <a name="apidoc.element.moment-timezone.tz.Zone"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>tz.Zone (packedString)](#apidoc.element.moment-timezone.tz.Zone)
- description and source-code
```javascript
function Zone(packedString) {
		if (packedString) {
			this._set(unpack(packedString));
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.unix"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>unix (input)](#apidoc.element.moment-timezone.unix)
- description and source-code
```javascript
function createUnix(input) {
    return createLocal(input * 1000);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.updateLocale"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>updateLocale (name, config)](#apidoc.element.moment-timezone.updateLocale)
- description and source-code
```javascript
function updateLocale(name, config) {
    if (config != null) {
        var locale, parentConfig = baseConfig;
        // MERGE
        if (locales[name] != null) {
            parentConfig = locales[name]._config;
        }
        config = mergeConfigs(parentConfig, config);
        locale = new Locale(config);
        locale.parentLocale = locales[name];
        locales[name] = locale;

        // backwards compat for now: also set the locale
        getSetGlobalLocale(name);
    } else {
        // pass null for config to unupdate, useful for tests
        if (locales[name] != null) {
            if (locales[name].parentLocale != null) {
                locales[name] = locales[name].parentLocale;
            } else if (locales[name] != null) {
                delete locales[name];
            }
        }
    }
    return locales[name];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.updateOffset"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>updateOffset (mom, keepTime)](#apidoc.element.moment-timezone.updateOffset)
- description and source-code
```javascript
updateOffset = function (mom, keepTime) {
		var zone = moment.defaultZone,
			offset;

		if (mom._z === undefined) {
			if (zone && needsOffset(mom) && !mom._isUTC) {
				mom._d = moment.utc(mom._a)._d;
				mom.utc().add(zone.parse(mom), 'minutes');
			}
			mom._z = zone;
		}
		if (mom._z) {
			offset = mom._z.offset(mom);
			if (Math.abs(offset) < 16) {
				offset = offset / 60;
			}
			if (mom.utcOffset !== undefined) {
				mom.utcOffset(-offset, keepTime);
			} else {
				mom.zone(offset, keepTime);
			}
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.utc"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>utc (input, format, locale, strict)](#apidoc.element.moment-timezone.utc)
- description and source-code
```javascript
function createUTC(input, format, locale, strict) {
    return createLocalOrUTC(input, format, locale, strict, true).utc();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.weekdays"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>weekdays (localeSorted, format, index)](#apidoc.element.moment-timezone.weekdays)
- description and source-code
```javascript
function listWeekdays(localeSorted, format, index) {
    return listWeekdaysImpl(localeSorted, format, index, 'weekdays');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.weekdaysMin"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>weekdaysMin (localeSorted, format, index)](#apidoc.element.moment-timezone.weekdaysMin)
- description and source-code
```javascript
function listWeekdaysMin(localeSorted, format, index) {
    return listWeekdaysImpl(localeSorted, format, index, 'weekdaysMin');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.weekdaysShort"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>weekdaysShort (localeSorted, format, index)](#apidoc.element.moment-timezone.weekdaysShort)
- description and source-code
```javascript
function listWeekdaysShort(localeSorted, format, index) {
    return listWeekdaysImpl(localeSorted, format, index, 'weekdaysShort');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.moment-timezone.duration"></a>[module moment-timezone.duration](#apidoc.module.moment-timezone.duration)

#### <a name="apidoc.element.moment-timezone.duration.duration"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>duration (input, key)](#apidoc.element.moment-timezone.duration.duration)
- description and source-code
```javascript
function createDuration(input, key) {
    var duration = input,
        // matching against regexp is expensive, do it on demand
        match = null,
        sign,
        ret,
        diffRes;

    if (isDuration(input)) {
        duration = {
            ms : input._milliseconds,
            d  : input._days,
            M  : input._months
        };
    } else if (isNumber(input)) {
        duration = {};
        if (key) {
            duration[key] = input;
        } else {
            duration.milliseconds = input;
        }
    } else if (!!(match = aspNetRegex.exec(input))) {
        sign = (match[1] === '-') ? -1 : 1;
        duration = {
            y  : 0,
            d  : toInt(match[DATE])                         * sign,
            h  : toInt(match[HOUR])                         * sign,
            m  : toInt(match[MINUTE])                       * sign,
            s  : toInt(match[SECOND])                       * sign,
            ms : toInt(absRound(match[MILLISECOND] * 1000)) * sign // the millisecond decimal point is included in the match
        };
    } else if (!!(match = isoRegex.exec(input))) {
        sign = (match[1] === '-') ? -1 : 1;
        duration = {
            y : parseIso(match[2], sign),
            M : parseIso(match[3], sign),
            w : parseIso(match[4], sign),
            d : parseIso(match[5], sign),
            h : parseIso(match[6], sign),
            m : parseIso(match[7], sign),
            s : parseIso(match[8], sign)
        };
    } else if (duration == null) {// checks for null or undefined
        duration = {};
    } else if (typeof duration === 'object' && ('from' in duration || 'to' in duration)) {
        diffRes = momentsDifference(createLocal(duration.from), createLocal(duration.to));

        duration = {};
        duration.ms = diffRes.milliseconds;
        duration.M = diffRes.months;
    }

    ret = new Duration(duration);

    if (isDuration(input) && hasOwnProp(input, '_locale')) {
        ret._locale = input._locale;
    }

    return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.invalid"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.</span>invalid ()](#apidoc.element.moment-timezone.duration.invalid)
- description and source-code
```javascript
function createInvalid$1() {
    return createDuration(NaN);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.moment-timezone.duration.fn"></a>[module moment-timezone.duration.fn](#apidoc.module.moment-timezone.duration.fn)

#### <a name="apidoc.element.moment-timezone.duration.fn._bubble"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>_bubble ()](#apidoc.element.moment-timezone.duration.fn._bubble)
- description and source-code
```javascript
function bubble() {
    var milliseconds = this._milliseconds;
    var days         = this._days;
    var months       = this._months;
    var data         = this._data;
    var seconds, minutes, hours, years, monthsFromDays;

    // if we have a mix of positive and negative values, bubble down first
    // check: https://github.com/moment/moment/issues/2166
    if (!((milliseconds >= 0 && days >= 0 && months >= 0) ||
            (milliseconds <= 0 && days <= 0 && months <= 0))) {
        milliseconds += absCeil(monthsToDays(months) + days) * 864e5;
        days = 0;
        months = 0;
    }

    // The following code bubbles up values, see the tests for
    // examples of what that means.
    data.milliseconds = milliseconds % 1000;

    seconds           = absFloor(milliseconds / 1000);
    data.seconds      = seconds % 60;

    minutes           = absFloor(seconds / 60);
    data.minutes      = minutes % 60;

    hours             = absFloor(minutes / 60);
    data.hours        = hours % 24;

    days += absFloor(hours / 24);

    // convert days to months
    monthsFromDays = absFloor(daysToMonths(days));
    months += monthsFromDays;
    days -= absCeil(monthsToDays(monthsFromDays));

    // 12 months -> 1 year
    years = absFloor(months / 12);
    months %= 12;

    data.days   = days;
    data.months = months;
    data.years  = years;

    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.abs"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>abs ()](#apidoc.element.moment-timezone.duration.fn.abs)
- description and source-code
```javascript
function abs() {
    var data           = this._data;

    this._milliseconds = mathAbs(this._milliseconds);
    this._days         = mathAbs(this._days);
    this._months       = mathAbs(this._months);

    data.milliseconds  = mathAbs(data.milliseconds);
    data.seconds       = mathAbs(data.seconds);
    data.minutes       = mathAbs(data.minutes);
    data.hours         = mathAbs(data.hours);
    data.months        = mathAbs(data.months);
    data.years         = mathAbs(data.years);

    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.add"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>add (input, value)](#apidoc.element.moment-timezone.duration.fn.add)
- description and source-code
```javascript
function add$1(input, value) {
    return addSubtract$1(this, input, value, 1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.as"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>as (units)](#apidoc.element.moment-timezone.duration.fn.as)
- description and source-code
```javascript
function as(units) {
    if (!this.isValid()) {
        return NaN;
    }
    var days;
    var months;
    var milliseconds = this._milliseconds;

    units = normalizeUnits(units);

    if (units === 'month' || units === 'year') {
        days   = this._days   + milliseconds / 864e5;
        months = this._months + daysToMonths(days);
        return units === 'month' ? months : months / 12;
    } else {
        // handle milliseconds separately because of floating point math errors (issue #1867)
        days = this._days + Math.round(monthsToDays(this._months));
        switch (units) {
            case 'week'   : return days / 7     + milliseconds / 6048e5;
            case 'day'    : return days         + milliseconds / 864e5;
            case 'hour'   : return days * 24    + milliseconds / 36e5;
            case 'minute' : return days * 1440  + milliseconds / 6e4;
            case 'second' : return days * 86400 + milliseconds / 1000;
            // Math.floor prevents floating point math errors here
            case 'millisecond': return Math.floor(days * 864e5) + milliseconds;
            default: throw new Error('Unknown unit ' + units);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.asDays"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>asDays ()](#apidoc.element.moment-timezone.duration.fn.asDays)
- description and source-code
```javascript
asDays = function () {
    return this.as(alias);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.asHours"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>asHours ()](#apidoc.element.moment-timezone.duration.fn.asHours)
- description and source-code
```javascript
asHours = function () {
    return this.as(alias);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.asMilliseconds"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>asMilliseconds ()](#apidoc.element.moment-timezone.duration.fn.asMilliseconds)
- description and source-code
```javascript
asMilliseconds = function () {
    return this.as(alias);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.asMinutes"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>asMinutes ()](#apidoc.element.moment-timezone.duration.fn.asMinutes)
- description and source-code
```javascript
asMinutes = function () {
    return this.as(alias);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.asMonths"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>asMonths ()](#apidoc.element.moment-timezone.duration.fn.asMonths)
- description and source-code
```javascript
asMonths = function () {
    return this.as(alias);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.asSeconds"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>asSeconds ()](#apidoc.element.moment-timezone.duration.fn.asSeconds)
- description and source-code
```javascript
asSeconds = function () {
    return this.as(alias);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.asWeeks"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>asWeeks ()](#apidoc.element.moment-timezone.duration.fn.asWeeks)
- description and source-code
```javascript
asWeeks = function () {
    return this.as(alias);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.asYears"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>asYears ()](#apidoc.element.moment-timezone.duration.fn.asYears)
- description and source-code
```javascript
asYears = function () {
    return this.as(alias);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.days"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>days ()](#apidoc.element.moment-timezone.duration.fn.days)
- description and source-code
```javascript
days = function () {
    return this.isValid() ? this._data[name] : NaN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.get"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>get (units)](#apidoc.element.moment-timezone.duration.fn.get)
- description and source-code
```javascript
function get$2(units) {
    units = normalizeUnits(units);
    return this.isValid() ? this[units + 's']() : NaN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.hours"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>hours ()](#apidoc.element.moment-timezone.duration.fn.hours)
- description and source-code
```javascript
hours = function () {
    return this.isValid() ? this._data[name] : NaN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.humanize"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>humanize (withSuffix)](#apidoc.element.moment-timezone.duration.fn.humanize)
- description and source-code
```javascript
function humanize(withSuffix) {
    if (!this.isValid()) {
        return this.localeData().invalidDate();
    }

    var locale = this.localeData();
    var output = relativeTime$1(this, !withSuffix, locale);

    if (withSuffix) {
        output = locale.pastFuture(+this, output);
    }

    return locale.postformat(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.isValid"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>isValid ()](#apidoc.element.moment-timezone.duration.fn.isValid)
- description and source-code
```javascript
function isValid$1() {
    return this._isValid;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.lang"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>lang ()](#apidoc.element.moment-timezone.duration.fn.lang)
- description and source-code
```javascript
lang = function () {
    if (hooks.deprecationHandler != null) {
        hooks.deprecationHandler(null, msg);
    }
    if (firstTime) {
        var args = [];
        var arg;
        for (var i = 0; i < arguments.length; i++) {
            arg = '';
            if (typeof arguments[i] === 'object') {
                arg += '\n[' + i + '] ';
                for (var key in arguments[0]) {
                    arg += key + ': ' + arguments[0][key] + ', ';
                }
                arg = arg.slice(0, -2); // Remove trailing comma and space
            } else {
                arg = arguments[i];
            }
            args.push(arg);
        }
        warn(msg + '\nArguments: ' + Array.prototype.slice.call(args).join('') + '\n' + (new Error()).stack);
        firstTime = false;
    }
    return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.locale"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>locale (key)](#apidoc.element.moment-timezone.duration.fn.locale)
- description and source-code
```javascript
function locale(key) {
    var newLocaleData;

    if (key === undefined) {
        return this._locale._abbr;
    } else {
        newLocaleData = getLocale(key);
        if (newLocaleData != null) {
            this._locale = newLocaleData;
        }
        return this;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.localeData"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>localeData ()](#apidoc.element.moment-timezone.duration.fn.localeData)
- description and source-code
```javascript
function localeData() {
    return this._locale;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.milliseconds"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>milliseconds ()](#apidoc.element.moment-timezone.duration.fn.milliseconds)
- description and source-code
```javascript
milliseconds = function () {
    return this.isValid() ? this._data[name] : NaN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.minutes"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>minutes ()](#apidoc.element.moment-timezone.duration.fn.minutes)
- description and source-code
```javascript
minutes = function () {
    return this.isValid() ? this._data[name] : NaN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.months"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>months ()](#apidoc.element.moment-timezone.duration.fn.months)
- description and source-code
```javascript
months = function () {
    return this.isValid() ? this._data[name] : NaN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.seconds"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>seconds ()](#apidoc.element.moment-timezone.duration.fn.seconds)
- description and source-code
```javascript
seconds = function () {
    return this.isValid() ? this._data[name] : NaN;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.subtract"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>subtract (input, value)](#apidoc.element.moment-timezone.duration.fn.subtract)
- description and source-code
```javascript
function subtract$1(input, value) {
    return addSubtract$1(this, input, value, -1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.toISOString"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>toISOString ()](#apidoc.element.moment-timezone.duration.fn.toISOString)
- description and source-code
```javascript
function toISOString$1() {
    // for ISO strings we do not use the normal bubbling rules:
    //  * milliseconds bubble up until they become hours
    //  * days do not bubble at all
    //  * months bubble up until they become years
    // This is because there is no context-free conversion between hours and days
    // (think of clock changes)
    // and also not between days and months (28-31 days per month)
    if (!this.isValid()) {
        return this.localeData().invalidDate();
    }

    var seconds = abs$1(this._milliseconds) / 1000;
    var days         = abs$1(this._days);
    var months       = abs$1(this._months);
    var minutes, hours, years;

    // 3600 seconds -> 60 minutes -> 1 hour
    minutes           = absFloor(seconds / 60);
    hours             = absFloor(minutes / 60);
    seconds %= 60;
    minutes %= 60;

    // 12 months -> 1 year
    years  = absFloor(months / 12);
    months %= 12;


    // inspired by https://github.com/dordille/moment-isoduration/blob/master/moment.isoduration.js
    var Y = years;
    var M = months;
    var D = days;
    var h = hours;
    var m = minutes;
    var s = seconds;
    var total = this.asSeconds();

    if (!total) {
        // this is the same as C#'s (Noda) and python (isodate)...
        // but not other JS (goog.date)
        return 'P0D';
    }

    return (total < 0 ? '-' : '') +
        'P' +
        (Y ? Y + 'Y' : '') +
        (M ? M + 'M' : '') +
        (D ? D + 'D' : '') +
        ((h || m || s) ? 'T' : '') +
        (h ? h + 'H' : '') +
        (m ? m + 'M' : '') +
        (s ? s + 'S' : '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.toIsoString"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>toIsoString ()](#apidoc.element.moment-timezone.duration.fn.toIsoString)
- description and source-code
```javascript
toIsoString = function () {
    if (hooks.deprecationHandler != null) {
        hooks.deprecationHandler(null, msg);
    }
    if (firstTime) {
        var args = [];
        var arg;
        for (var i = 0; i < arguments.length; i++) {
            arg = '';
            if (typeof arguments[i] === 'object') {
                arg += '\n[' + i + '] ';
                for (var key in arguments[0]) {
                    arg += key + ': ' + arguments[0][key] + ', ';
                }
                arg = arg.slice(0, -2); // Remove trailing comma and space
            } else {
                arg = arguments[i];
            }
            args.push(arg);
        }
        warn(msg + '\nArguments: ' + Array.prototype.slice.call(args).join('') + '\n' + (new Error()).stack);
        firstTime = false;
    }
    return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.toJSON"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>toJSON ()](#apidoc.element.moment-timezone.duration.fn.toJSON)
- description and source-code
```javascript
function toISOString$1() {
    // for ISO strings we do not use the normal bubbling rules:
    //  * milliseconds bubble up until they become hours
    //  * days do not bubble at all
    //  * months bubble up until they become years
    // This is because there is no context-free conversion between hours and days
    // (think of clock changes)
    // and also not between days and months (28-31 days per month)
    if (!this.isValid()) {
        return this.localeData().invalidDate();
    }

    var seconds = abs$1(this._milliseconds) / 1000;
    var days         = abs$1(this._days);
    var months       = abs$1(this._months);
    var minutes, hours, years;

    // 3600 seconds -> 60 minutes -> 1 hour
    minutes           = absFloor(seconds / 60);
    hours             = absFloor(minutes / 60);
    seconds %= 60;
    minutes %= 60;

    // 12 months -> 1 year
    years  = absFloor(months / 12);
    months %= 12;


    // inspired by https://github.com/dordille/moment-isoduration/blob/master/moment.isoduration.js
    var Y = years;
    var M = months;
    var D = days;
    var h = hours;
    var m = minutes;
    var s = seconds;
    var total = this.asSeconds();

    if (!total) {
        // this is the same as C#'s (Noda) and python (isodate)...
        // but not other JS (goog.date)
        return 'P0D';
    }

    return (total < 0 ? '-' : '') +
        'P' +
        (Y ? Y + 'Y' : '') +
        (M ? M + 'M' : '') +
        (D ? D + 'D' : '') +
        ((h || m || s) ? 'T' : '') +
        (h ? h + 'H' : '') +
        (m ? m + 'M' : '') +
        (s ? s + 'S' : '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.toString"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>toString ()](#apidoc.element.moment-timezone.duration.fn.toString)
- description and source-code
```javascript
function toISOString$1() {
    // for ISO strings we do not use the normal bubbling rules:
    //  * milliseconds bubble up until they become hours
    //  * days do not bubble at all
    //  * months bubble up until they become years
    // This is because there is no context-free conversion between hours and days
    // (think of clock changes)
    // and also not between days and months (28-31 days per month)
    if (!this.isValid()) {
        return this.localeData().invalidDate();
    }

    var seconds = abs$1(this._milliseconds) / 1000;
    var days         = abs$1(this._days);
    var months       = abs$1(this._months);
    var minutes, hours, years;

    // 3600 seconds -> 60 minutes -> 1 hour
    minutes           = absFloor(seconds / 60);
    hours             = absFloor(minutes / 60);
    seconds %= 60;
    minutes %= 60;

    // 12 months -> 1 year
    years  = absFloor(months / 12);
    months %= 12;


    // inspired by https://github.com/dordille/moment-isoduration/blob/master/moment.isoduration.js
    var Y = years;
    var M = months;
    var D = days;
    var h = hours;
    var m = minutes;
    var s = seconds;
    var total = this.asSeconds();

    if (!total) {
        // this is the same as C#'s (Noda) and python (isodate)...
        // but not other JS (goog.date)
        return 'P0D';
    }

    return (total < 0 ? '-' : '') +
        'P' +
        (Y ? Y + 'Y' : '') +
        (M ? M + 'M' : '') +
        (D ? D + 'D' : '') +
        ((h || m || s) ? 'T' : '') +
        (h ? h + 'H' : '') +
        (m ? m + 'M' : '') +
        (s ? s + 'S' : '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.valueOf"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>valueOf ()](#apidoc.element.moment-timezone.duration.fn.valueOf)
- description and source-code
```javascript
function valueOf$1() {
    if (!this.isValid()) {
        return NaN;
    }
    return (
        this._milliseconds +
        this._days * 864e5 +
        (this._months % 12) * 2592e6 +
        toInt(this._months / 12) * 31536e6
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.weeks"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>weeks ()](#apidoc.element.moment-timezone.duration.fn.weeks)
- description and source-code
```javascript
function weeks() {
    return absFloor(this.days() / 7);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.duration.fn.years"></a>[function <span class="apidocSignatureSpan">moment-timezone.duration.fn.</span>years ()](#apidoc.element.moment-timezone.duration.fn.years)
- description and source-code
```javascript
years = function () {
    return this.isValid() ? this._data[name] : NaN;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.moment-timezone.fn"></a>[module moment-timezone.fn](#apidoc.module.moment-timezone.fn)

#### <a name="apidoc.element.moment-timezone.fn.add"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>add (val, period)](#apidoc.element.moment-timezone.fn.add)
- description and source-code
```javascript
add = function (val, period) {
    var dur, tmp;
    //invert the arguments, but complain about it
    if (period !== null && !isNaN(+period)) {
        deprecateSimple(name, 'moment().' + name  + '(period, number) is deprecated. Please use moment().' + name + '(number, period
). ' +
        'See http://momentjs.com/guides/#/warnings/add-inverted-param/ for more info.');
        tmp = val; val = period; period = tmp;
    }

    val = typeof val === 'string' ? +val : val;
    dur = createDuration(val, period);
    addSubtract(this, dur, direction);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.calendar"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>calendar (time, formats)](#apidoc.element.moment-timezone.fn.calendar)
- description and source-code
```javascript
function calendar$1(time, formats) {
    // We want to compare the start of today, vs this.
    // Getting start-of-today depends on whether we're local/utc/offset or not.
    var now = time || createLocal(),
        sod = cloneWithOffset(now, this).startOf('day'),
        format = hooks.calendarFormat(this, sod) || 'sameElse';

    var output = formats && (isFunction(formats[format]) ? formats[format].call(this, now) : formats[format]);

    return this.format(output || this.localeData().calendar(format, this, createLocal(now)));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.clone"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>clone ()](#apidoc.element.moment-timezone.fn.clone)
- description and source-code
```javascript
function clone() {
    return new Moment(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.creationData"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>creationData ()](#apidoc.element.moment-timezone.fn.creationData)
- description and source-code
```javascript
function creationData() {
    return {
        input: this._i,
        format: this._f,
        locale: this._locale,
        isUTC: this._isUTC,
        strict: this._strict
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.date"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>date (value)](#apidoc.element.moment-timezone.fn.date)
- description and source-code
```javascript
date = function (value) {
    if (value != null) {
        set$1(this, unit, value);
        hooks.updateOffset(this, keepTime);
        return this;
    } else {
        return get(this, unit);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.dates"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>dates ()](#apidoc.element.moment-timezone.fn.dates)
- description and source-code
```javascript
dates = function () {
    if (hooks.deprecationHandler != null) {
        hooks.deprecationHandler(null, msg);
    }
    if (firstTime) {
        var args = [];
        var arg;
        for (var i = 0; i < arguments.length; i++) {
            arg = '';
            if (typeof arguments[i] === 'object') {
                arg += '\n[' + i + '] ';
                for (var key in arguments[0]) {
                    arg += key + ': ' + arguments[0][key] + ', ';
                }
                arg = arg.slice(0, -2); // Remove trailing comma and space
            } else {
                arg = arguments[i];
            }
            args.push(arg);
        }
        warn(msg + '\nArguments: ' + Array.prototype.slice.call(args).join('') + '\n' + (new Error()).stack);
        firstTime = false;
    }
    return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.day"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>day (input)](#apidoc.element.moment-timezone.fn.day)
- description and source-code
```javascript
function getSetDayOfWeek(input) {
    if (!this.isValid()) {
        return input != null ? this : NaN;
    }
    var day = this._isUTC ? this._d.getUTCDay() : this._d.getDay();
    if (input != null) {
        input = parseWeekday(input, this.localeData());
        return this.add(input - day, 'd');
    } else {
        return day;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.dayOfYear"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>dayOfYear (input)](#apidoc.element.moment-timezone.fn.dayOfYear)
- description and source-code
```javascript
function getSetDayOfYear(input) {
    var dayOfYear = Math.round((this.clone().startOf('day') - this.clone().startOf('year')) / 864e5) + 1;
    return input == null ? dayOfYear : this.add((input - dayOfYear), 'd');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.days"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>days (input)](#apidoc.element.moment-timezone.fn.days)
- description and source-code
```javascript
function getSetDayOfWeek(input) {
    if (!this.isValid()) {
        return input != null ? this : NaN;
    }
    var day = this._isUTC ? this._d.getUTCDay() : this._d.getDay();
    if (input != null) {
        input = parseWeekday(input, this.localeData());
        return this.add(input - day, 'd');
    } else {
        return day;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.daysInMonth"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>daysInMonth ()](#apidoc.element.moment-timezone.fn.daysInMonth)
- description and source-code
```javascript
function getDaysInMonth() {
    return daysInMonth(this.year(), this.month());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.diff"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>diff (input, units, asFloat)](#apidoc.element.moment-timezone.fn.diff)
- description and source-code
```javascript
function diff(input, units, asFloat) {
    var that,
        zoneDelta,
        delta, output;

    if (!this.isValid()) {
        return NaN;
    }

    that = cloneWithOffset(input, this);

    if (!that.isValid()) {
        return NaN;
    }

    zoneDelta = (that.utcOffset() - this.utcOffset()) * 6e4;

    units = normalizeUnits(units);

    if (units === 'year' || units === 'month' || units === 'quarter') {
        output = monthDiff(this, that);
        if (units === 'quarter') {
            output = output / 3;
        } else if (units === 'year') {
            output = output / 12;
        }
    } else {
        delta = this - that;
        output = units === 'second' ? delta / 1e3 : // 1000
            units === 'minute' ? delta / 6e4 : // 1000 * 60
            units === 'hour' ? delta / 36e5 : // 1000 * 60 * 60
            units === 'day' ? (delta - zoneDelta) / 864e5 : // 1000 * 60 * 60 * 24, negate dst
            units === 'week' ? (delta - zoneDelta) / 6048e5 : // 1000 * 60 * 60 * 24 * 7, negate dst
            delta;
    }
    return asFloat ? output : absFloor(output);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.endOf"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>endOf (units)](#apidoc.element.moment-timezone.fn.endOf)
- description and source-code
```javascript
function endOf(units) {
    units = normalizeUnits(units);
    if (units === undefined || units === 'millisecond') {
        return this;
    }

    // 'date' is an alias for 'day', so it should be considered as such.
    if (units === 'date') {
        units = 'day';
    }

    return this.startOf(units).add(1, (units === 'isoWeek' ? 'week' : units)).subtract(1, 'ms');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.format"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>format (inputString)](#apidoc.element.moment-timezone.fn.format)
- description and source-code
```javascript
function format(inputString) {
    if (!inputString) {
        inputString = this.isUtc() ? hooks.defaultFormatUtc : hooks.defaultFormat;
    }
    var output = formatMoment(this, inputString);
    return this.localeData().postformat(output);
}
```
- example usage
```shell
...

[![NPM version][npm-version-image]][npm-url] [![NPM downloads][npm-downloads-image]][npm-url] [![MIT License][license-image]][license
-url] [![Build Status][travis-image]][travis-url]

IANA Time Zone Database + [Moment.js](http://momentjs.com).

'''js
var june = moment("2014-06-01T12:00:00Z");
june.tz('America/Los_Angeles').format('ha z'); // 5am PDT
june.tz('America/New_York').format('ha z');    // 8am EDT
june.tz('Asia/Tokyo').format('ha z');          // 9pm JST
june.tz('Australia/Sydney').format('ha z');    // 10pm EST

var dec = moment("2014-12-01T12:00:00Z");
dec.tz('America/Los_Angeles').format('ha z');  // 4am PST
dec.tz('America/New_York').format('ha z');     // 7am EST
...
```

#### <a name="apidoc.element.moment-timezone.fn.from"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>from (time, withoutSuffix)](#apidoc.element.moment-timezone.fn.from)
- description and source-code
```javascript
function from(time, withoutSuffix) {
    if (this.isValid() &&
            ((isMoment(time) && time.isValid()) ||
             createLocal(time).isValid())) {
        return createDuration({to: this, from: time}).locale(this.locale()).humanize(!withoutSuffix);
    } else {
        return this.localeData().invalidDate();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.fromNow"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>fromNow (withoutSuffix)](#apidoc.element.moment-timezone.fn.fromNow)
- description and source-code
```javascript
function fromNow(withoutSuffix) {
    return this.from(createLocal(), withoutSuffix);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.get"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>get (units)](#apidoc.element.moment-timezone.fn.get)
- description and source-code
```javascript
function stringGet(units) {
    units = normalizeUnits(units);
    if (isFunction(this[units])) {
        return this[units]();
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.hasAlignedHourOffset"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>hasAlignedHourOffset (input)](#apidoc.element.moment-timezone.fn.hasAlignedHourOffset)
- description and source-code
```javascript
function hasAlignedHourOffset(input) {
    if (!this.isValid()) {
        return false;
    }
    input = input ? createLocal(input).utcOffset() : 0;

    return (this.utcOffset() - input) % 60 === 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.hour"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>hour (value)](#apidoc.element.moment-timezone.fn.hour)
- description and source-code
```javascript
hour = function (value) {
    if (value != null) {
        set$1(this, unit, value);
        hooks.updateOffset(this, keepTime);
        return this;
    } else {
        return get(this, unit);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.hours"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>hours (value)](#apidoc.element.moment-timezone.fn.hours)
- description and source-code
```javascript
hours = function (value) {
    if (value != null) {
        set$1(this, unit, value);
        hooks.updateOffset(this, keepTime);
        return this;
    } else {
        return get(this, unit);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.inspect"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>inspect ()](#apidoc.element.moment-timezone.fn.inspect)
- description and source-code
```javascript
function inspect() {
    if (!this.isValid()) {
        return 'moment.invalid(/* ' + this._i + ' */)';
    }
    var func = 'moment';
    var zone = '';
    if (!this.isLocal()) {
        func = this.utcOffset() === 0 ? 'moment.utc' : 'moment.parseZone';
        zone = 'Z';
    }
    var prefix = '[' + func + '("]';
    var year = (0 <= this.year() && this.year() <= 9999) ? 'YYYY' : 'YYYYYY';
    var datetime = '-MM-DD[T]HH:mm:ss.SSS';
    var suffix = zone + '[")]';

    return this.format(prefix + year + datetime + suffix);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.invalidAt"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>invalidAt ()](#apidoc.element.moment-timezone.fn.invalidAt)
- description and source-code
```javascript
function invalidAt() {
    return getParsingFlags(this).overflow;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.isAfter"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isAfter (input, units)](#apidoc.element.moment-timezone.fn.isAfter)
- description and source-code
```javascript
function isAfter(input, units) {
    var localInput = isMoment(input) ? input : createLocal(input);
    if (!(this.isValid() && localInput.isValid())) {
        return false;
    }
    units = normalizeUnits(!isUndefined(units) ? units : 'millisecond');
    if (units === 'millisecond') {
        return this.valueOf() > localInput.valueOf();
    } else {
        return localInput.valueOf() < this.clone().startOf(units).valueOf();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.isBefore"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isBefore (input, units)](#apidoc.element.moment-timezone.fn.isBefore)
- description and source-code
```javascript
function isBefore(input, units) {
    var localInput = isMoment(input) ? input : createLocal(input);
    if (!(this.isValid() && localInput.isValid())) {
        return false;
    }
    units = normalizeUnits(!isUndefined(units) ? units : 'millisecond');
    if (units === 'millisecond') {
        return this.valueOf() < localInput.valueOf();
    } else {
        return this.clone().endOf(units).valueOf() < localInput.valueOf();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.isBetween"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isBetween (from, to, units, inclusivity)](#apidoc.element.moment-timezone.fn.isBetween)
- description and source-code
```javascript
function isBetween(from, to, units, inclusivity) {
    inclusivity = inclusivity || '()';
    return (inclusivity[0] === '(' ? this.isAfter(from, units) : !this.isBefore(from, units)) &&
        (inclusivity[1] === ')' ? this.isBefore(to, units) : !this.isAfter(to, units));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.isDST"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isDST ()](#apidoc.element.moment-timezone.fn.isDST)
- description and source-code
```javascript
function isDaylightSavingTime() {
    return (
        this.utcOffset() > this.clone().month(0).utcOffset() ||
        this.utcOffset() > this.clone().month(5).utcOffset()
    );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.isDSTShifted"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isDSTShifted ()](#apidoc.element.moment-timezone.fn.isDSTShifted)
- description and source-code
```javascript
isDSTShifted = function () {
    if (hooks.deprecationHandler != null) {
        hooks.deprecationHandler(null, msg);
    }
    if (firstTime) {
        var args = [];
        var arg;
        for (var i = 0; i < arguments.length; i++) {
            arg = '';
            if (typeof arguments[i] === 'object') {
                arg += '\n[' + i + '] ';
                for (var key in arguments[0]) {
                    arg += key + ': ' + arguments[0][key] + ', ';
                }
                arg = arg.slice(0, -2); // Remove trailing comma and space
            } else {
                arg = arguments[i];
            }
            args.push(arg);
        }
        warn(msg + '\nArguments: ' + Array.prototype.slice.call(args).join('') + '\n' + (new Error()).stack);
        firstTime = false;
    }
    return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.isLeapYear"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isLeapYear ()](#apidoc.element.moment-timezone.fn.isLeapYear)
- description and source-code
```javascript
function getIsLeapYear() {
    return isLeapYear(this.year());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.isLocal"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isLocal ()](#apidoc.element.moment-timezone.fn.isLocal)
- description and source-code
```javascript
function isLocal() {
    return this.isValid() ? !this._isUTC : false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.isSame"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isSame (input, units)](#apidoc.element.moment-timezone.fn.isSame)
- description and source-code
```javascript
function isSame(input, units) {
    var localInput = isMoment(input) ? input : createLocal(input),
        inputMs;
    if (!(this.isValid() && localInput.isValid())) {
        return false;
    }
    units = normalizeUnits(units || 'millisecond');
    if (units === 'millisecond') {
        return this.valueOf() === localInput.valueOf();
    } else {
        inputMs = localInput.valueOf();
        return this.clone().startOf(units).valueOf() <= inputMs && inputMs <= this.clone().endOf(units).valueOf();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.isSameOrAfter"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isSameOrAfter (input, units)](#apidoc.element.moment-timezone.fn.isSameOrAfter)
- description and source-code
```javascript
function isSameOrAfter(input, units) {
    return this.isSame(input, units) || this.isAfter(input,units);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.isSameOrBefore"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isSameOrBefore (input, units)](#apidoc.element.moment-timezone.fn.isSameOrBefore)
- description and source-code
```javascript
function isSameOrBefore(input, units) {
    return this.isSame(input, units) || this.isBefore(input,units);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.isUTC"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isUTC ()](#apidoc.element.moment-timezone.fn.isUTC)
- description and source-code
```javascript
function isUtc() {
    return this.isValid() ? this._isUTC && this._offset === 0 : false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.isUtc"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isUtc ()](#apidoc.element.moment-timezone.fn.isUtc)
- description and source-code
```javascript
function isUtc() {
    return this.isValid() ? this._isUTC && this._offset === 0 : false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.isUtcOffset"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isUtcOffset ()](#apidoc.element.moment-timezone.fn.isUtcOffset)
- description and source-code
```javascript
function isUtcOffset() {
    return this.isValid() ? this._isUTC : false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.isValid"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isValid ()](#apidoc.element.moment-timezone.fn.isValid)
- description and source-code
```javascript
function isValid$2() {
    return isValid(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.isoWeek"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isoWeek (input)](#apidoc.element.moment-timezone.fn.isoWeek)
- description and source-code
```javascript
function getSetISOWeek(input) {
    var week = weekOfYear(this, 1, 4).week;
    return input == null ? week : this.add((input - week) * 7, 'd');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.isoWeekYear"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isoWeekYear (input)](#apidoc.element.moment-timezone.fn.isoWeekYear)
- description and source-code
```javascript
function getSetISOWeekYear(input) {
    return getSetWeekYearHelper.call(this,
            input, this.isoWeek(), this.isoWeekday(), 1, 4);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.isoWeekday"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isoWeekday (input)](#apidoc.element.moment-timezone.fn.isoWeekday)
- description and source-code
```javascript
function getSetISODayOfWeek(input) {
    if (!this.isValid()) {
        return input != null ? this : NaN;
    }

    // behaves the same as moment#day except
    // as a getter, returns 7 instead of 0 (1-7 range instead of 0-6)
    // as a setter, sunday should belong to the previous week.

    if (input != null) {
        var weekday = parseIsoWeekday(input, this.localeData());
        return this.day(this.day() % 7 ? weekday : weekday - 7);
    } else {
        return this.day() || 7;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.isoWeeks"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isoWeeks (input)](#apidoc.element.moment-timezone.fn.isoWeeks)
- description and source-code
```javascript
function getSetISOWeek(input) {
    var week = weekOfYear(this, 1, 4).week;
    return input == null ? week : this.add((input - week) * 7, 'd');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.isoWeeksInYear"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>isoWeeksInYear ()](#apidoc.element.moment-timezone.fn.isoWeeksInYear)
- description and source-code
```javascript
function getISOWeeksInYear() {
    return weeksInYear(this.year(), 1, 4);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.lang"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>lang ()](#apidoc.element.moment-timezone.fn.lang)
- description and source-code
```javascript
lang = function () {
    if (hooks.deprecationHandler != null) {
        hooks.deprecationHandler(null, msg);
    }
    if (firstTime) {
        var args = [];
        var arg;
        for (var i = 0; i < arguments.length; i++) {
            arg = '';
            if (typeof arguments[i] === 'object') {
                arg += '\n[' + i + '] ';
                for (var key in arguments[0]) {
                    arg += key + ': ' + arguments[0][key] + ', ';
                }
                arg = arg.slice(0, -2); // Remove trailing comma and space
            } else {
                arg = arguments[i];
            }
            args.push(arg);
        }
        warn(msg + '\nArguments: ' + Array.prototype.slice.call(args).join('') + '\n' + (new Error()).stack);
        firstTime = false;
    }
    return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.local"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>local (keepLocalTime)](#apidoc.element.moment-timezone.fn.local)
- description and source-code
```javascript
function setOffsetToLocal(keepLocalTime) {
    if (this._isUTC) {
        this.utcOffset(0, keepLocalTime);
        this._isUTC = false;

        if (keepLocalTime) {
            this.subtract(getDateOffset(this), 'm');
        }
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.locale"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>locale (key)](#apidoc.element.moment-timezone.fn.locale)
- description and source-code
```javascript
function locale(key) {
    var newLocaleData;

    if (key === undefined) {
        return this._locale._abbr;
    } else {
        newLocaleData = getLocale(key);
        if (newLocaleData != null) {
            this._locale = newLocaleData;
        }
        return this;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.localeData"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>localeData ()](#apidoc.element.moment-timezone.fn.localeData)
- description and source-code
```javascript
function localeData() {
    return this._locale;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.max"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>max ()](#apidoc.element.moment-timezone.fn.max)
- description and source-code
```javascript
max = function () {
    if (hooks.deprecationHandler != null) {
        hooks.deprecationHandler(null, msg);
    }
    if (firstTime) {
        var args = [];
        var arg;
        for (var i = 0; i < arguments.length; i++) {
            arg = '';
            if (typeof arguments[i] === 'object') {
                arg += '\n[' + i + '] ';
                for (var key in arguments[0]) {
                    arg += key + ': ' + arguments[0][key] + ', ';
                }
                arg = arg.slice(0, -2); // Remove trailing comma and space
            } else {
                arg = arguments[i];
            }
            args.push(arg);
        }
        warn(msg + '\nArguments: ' + Array.prototype.slice.call(args).join('') + '\n' + (new Error()).stack);
        firstTime = false;
    }
    return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.millisecond"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>millisecond (value)](#apidoc.element.moment-timezone.fn.millisecond)
- description and source-code
```javascript
millisecond = function (value) {
    if (value != null) {
        set$1(this, unit, value);
        hooks.updateOffset(this, keepTime);
        return this;
    } else {
        return get(this, unit);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.milliseconds"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>milliseconds (value)](#apidoc.element.moment-timezone.fn.milliseconds)
- description and source-code
```javascript
milliseconds = function (value) {
    if (value != null) {
        set$1(this, unit, value);
        hooks.updateOffset(this, keepTime);
        return this;
    } else {
        return get(this, unit);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.min"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>min ()](#apidoc.element.moment-timezone.fn.min)
- description and source-code
```javascript
min = function () {
    if (hooks.deprecationHandler != null) {
        hooks.deprecationHandler(null, msg);
    }
    if (firstTime) {
        var args = [];
        var arg;
        for (var i = 0; i < arguments.length; i++) {
            arg = '';
            if (typeof arguments[i] === 'object') {
                arg += '\n[' + i + '] ';
                for (var key in arguments[0]) {
                    arg += key + ': ' + arguments[0][key] + ', ';
                }
                arg = arg.slice(0, -2); // Remove trailing comma and space
            } else {
                arg = arguments[i];
            }
            args.push(arg);
        }
        warn(msg + '\nArguments: ' + Array.prototype.slice.call(args).join('') + '\n' + (new Error()).stack);
        firstTime = false;
    }
    return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.minute"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>minute (value)](#apidoc.element.moment-timezone.fn.minute)
- description and source-code
```javascript
minute = function (value) {
    if (value != null) {
        set$1(this, unit, value);
        hooks.updateOffset(this, keepTime);
        return this;
    } else {
        return get(this, unit);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.minutes"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>minutes (value)](#apidoc.element.moment-timezone.fn.minutes)
- description and source-code
```javascript
minutes = function (value) {
    if (value != null) {
        set$1(this, unit, value);
        hooks.updateOffset(this, keepTime);
        return this;
    } else {
        return get(this, unit);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.month"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>month (value)](#apidoc.element.moment-timezone.fn.month)
- description and source-code
```javascript
function getSetMonth(value) {
    if (value != null) {
        setMonth(this, value);
        hooks.updateOffset(this, true);
        return this;
    } else {
        return get(this, 'Month');
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.months"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>months ()](#apidoc.element.moment-timezone.fn.months)
- description and source-code
```javascript
months = function () {
    if (hooks.deprecationHandler != null) {
        hooks.deprecationHandler(null, msg);
    }
    if (firstTime) {
        var args = [];
        var arg;
        for (var i = 0; i < arguments.length; i++) {
            arg = '';
            if (typeof arguments[i] === 'object') {
                arg += '\n[' + i + '] ';
                for (var key in arguments[0]) {
                    arg += key + ': ' + arguments[0][key] + ', ';
                }
                arg = arg.slice(0, -2); // Remove trailing comma and space
            } else {
                arg = arguments[i];
            }
            args.push(arg);
        }
        warn(msg + '\nArguments: ' + Array.prototype.slice.call(args).join('') + '\n' + (new Error()).stack);
        firstTime = false;
    }
    return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.parseZone"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>parseZone ()](#apidoc.element.moment-timezone.fn.parseZone)
- description and source-code
```javascript
function setOffsetToParsedOffset() {
    if (this._tzm != null) {
        this.utcOffset(this._tzm, false, true);
    } else if (typeof this._i === 'string') {
        var tZone = offsetFromString(matchOffset, this._i);
        if (tZone != null) {
            this.utcOffset(tZone);
        }
        else {
            this.utcOffset(0, true);
        }
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.parsingFlags"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>parsingFlags ()](#apidoc.element.moment-timezone.fn.parsingFlags)
- description and source-code
```javascript
function parsingFlags() {
    return extend({}, getParsingFlags(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.quarter"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>quarter (input)](#apidoc.element.moment-timezone.fn.quarter)
- description and source-code
```javascript
function getSetQuarter(input) {
    return input == null ? Math.ceil((this.month() + 1) / 3) : this.month((input - 1) * 3 + this.month() % 3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.quarters"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>quarters (input)](#apidoc.element.moment-timezone.fn.quarters)
- description and source-code
```javascript
function getSetQuarter(input) {
    return input == null ? Math.ceil((this.month() + 1) / 3) : this.month((input - 1) * 3 + this.month() % 3);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.second"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>second (value)](#apidoc.element.moment-timezone.fn.second)
- description and source-code
```javascript
second = function (value) {
    if (value != null) {
        set$1(this, unit, value);
        hooks.updateOffset(this, keepTime);
        return this;
    } else {
        return get(this, unit);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.seconds"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>seconds (value)](#apidoc.element.moment-timezone.fn.seconds)
- description and source-code
```javascript
seconds = function (value) {
    if (value != null) {
        set$1(this, unit, value);
        hooks.updateOffset(this, keepTime);
        return this;
    } else {
        return get(this, unit);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.set"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>set (units, value)](#apidoc.element.moment-timezone.fn.set)
- description and source-code
```javascript
function stringSet(units, value) {
    if (typeof units === 'object') {
        units = normalizeObjectUnits(units);
        var prioritized = getPrioritizedUnits(units);
        for (var i = 0; i < prioritized.length; i++) {
            this[prioritized[i].unit](units[prioritized[i].unit]);
        }
    } else {
        units = normalizeUnits(units);
        if (isFunction(this[units])) {
            return this[units](value);
        }
    }
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.startOf"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>startOf (units)](#apidoc.element.moment-timezone.fn.startOf)
- description and source-code
```javascript
function startOf(units) {
    units = normalizeUnits(units);
    // the following switch intentionally omits break keywords
    // to utilize falling through the cases.
    switch (units) {
        case 'year':
            this.month(0);
<span class="apidocCodeCommentSpan">            /* falls through */
</span>        case 'quarter':
        case 'month':
            this.date(1);
            /* falls through */
        case 'week':
        case 'isoWeek':
        case 'day':
        case 'date':
            this.hours(0);
            /* falls through */
        case 'hour':
            this.minutes(0);
            /* falls through */
        case 'minute':
            this.seconds(0);
            /* falls through */
        case 'second':
            this.milliseconds(0);
    }

    // weeks are a special case
    if (units === 'week') {
        this.weekday(0);
    }
    if (units === 'isoWeek') {
        this.isoWeekday(1);
    }

    // quarters are also special
    if (units === 'quarter') {
        this.month(Math.floor(this.month() / 3) * 3);
    }

    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.subtract"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>subtract (val, period)](#apidoc.element.moment-timezone.fn.subtract)
- description and source-code
```javascript
subtract = function (val, period) {
    var dur, tmp;
    //invert the arguments, but complain about it
    if (period !== null && !isNaN(+period)) {
        deprecateSimple(name, 'moment().' + name  + '(period, number) is deprecated. Please use moment().' + name + '(number, period
). ' +
        'See http://momentjs.com/guides/#/warnings/add-inverted-param/ for more info.');
        tmp = val; val = period; period = tmp;
    }

    val = typeof val === 'string' ? +val : val;
    dur = createDuration(val, period);
    addSubtract(this, dur, direction);
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.to"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>to (time, withoutSuffix)](#apidoc.element.moment-timezone.fn.to)
- description and source-code
```javascript
function to(time, withoutSuffix) {
    if (this.isValid() &&
            ((isMoment(time) && time.isValid()) ||
             createLocal(time).isValid())) {
        return createDuration({from: this, to: time}).locale(this.locale()).humanize(!withoutSuffix);
    } else {
        return this.localeData().invalidDate();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.toArray"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>toArray ()](#apidoc.element.moment-timezone.fn.toArray)
- description and source-code
```javascript
function toArray() {
    var m = this;
    return [m.year(), m.month(), m.date(), m.hour(), m.minute(), m.second(), m.millisecond()];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.toDate"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>toDate ()](#apidoc.element.moment-timezone.fn.toDate)
- description and source-code
```javascript
function toDate() {
    return new Date(this.valueOf());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.toISOString"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>toISOString ()](#apidoc.element.moment-timezone.fn.toISOString)
- description and source-code
```javascript
function toISOString() {
    if (!this.isValid()) {
        return null;
    }
    var m = this.clone().utc();
    if (m.year() < 0 || m.year() > 9999) {
        return formatMoment(m, 'YYYYYY-MM-DD[T]HH:mm:ss.SSS[Z]');
    }
    if (isFunction(Date.prototype.toISOString)) {
        // native implementation is ~50x faster, use it when we can
        return this.toDate().toISOString();
    }
    return formatMoment(m, 'YYYY-MM-DD[T]HH:mm:ss.SSS[Z]');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.toJSON"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>toJSON ()](#apidoc.element.moment-timezone.fn.toJSON)
- description and source-code
```javascript
function toJSON() {
    // new Date(NaN).toJSON() === null
    return this.isValid() ? this.toISOString() : null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.toNow"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>toNow (withoutSuffix)](#apidoc.element.moment-timezone.fn.toNow)
- description and source-code
```javascript
function toNow(withoutSuffix) {
    return this.to(createLocal(), withoutSuffix);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.toObject"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>toObject ()](#apidoc.element.moment-timezone.fn.toObject)
- description and source-code
```javascript
function toObject() {
    var m = this;
    return {
        years: m.year(),
        months: m.month(),
        date: m.date(),
        hours: m.hours(),
        minutes: m.minutes(),
        seconds: m.seconds(),
        milliseconds: m.milliseconds()
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.toString"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>toString ()](#apidoc.element.moment-timezone.fn.toString)
- description and source-code
```javascript
function toString() {
    return this.clone().locale('en').format('ddd MMM DD YYYY HH:mm:ss [GMT]ZZ');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.tz"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>tz (name)](#apidoc.element.moment-timezone.fn.tz)
- description and source-code
```javascript
tz = function (name) {
		if (name) {
			this._z = getZone(name);
			if (this._z) {
				moment.updateOffset(this);
			} else {
				logError("Moment Timezone has no data for " + name + ". See http://momentjs.com/timezone/docs/#/data-loading/.");
			}
			return this;
		}
		if (this._z) { return this._z.name; }
	}
```
- example usage
```shell
...

[![NPM version][npm-version-image]][npm-url] [![NPM downloads][npm-downloads-image]][npm-url] [![MIT License][license-image]][license
-url] [![Build Status][travis-image]][travis-url]

IANA Time Zone Database + [Moment.js](http://momentjs.com).

'''js
var june = moment("2014-06-01T12:00:00Z");
june.tz('America/Los_Angeles').format('ha z'); // 5am PDT
june.tz('America/New_York').format('ha z');    // 8am EDT
june.tz('Asia/Tokyo').format('ha z');          // 9pm JST
june.tz('Australia/Sydney').format('ha z');    // 10pm EST

var dec = moment("2014-12-01T12:00:00Z");
dec.tz('America/Los_Angeles').format('ha z');  // 4am PST
dec.tz('America/New_York').format('ha z');     // 7am EST
...
```

#### <a name="apidoc.element.moment-timezone.fn.unix"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>unix ()](#apidoc.element.moment-timezone.fn.unix)
- description and source-code
```javascript
function unix() {
    return Math.floor(this.valueOf() / 1000);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.utc"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>utc ()](#apidoc.element.moment-timezone.fn.utc)
- description and source-code
```javascript
utc = function () {
			this._z = null;
			return old.apply(this, arguments);
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.utcOffset"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>utcOffset (input, keepLocalTime, keepMinutes)](#apidoc.element.moment-timezone.fn.utcOffset)
- description and source-code
```javascript
function getSetOffset(input, keepLocalTime, keepMinutes) {
    var offset = this._offset || 0,
        localAdjust;
    if (!this.isValid()) {
        return input != null ? this : NaN;
    }
    if (input != null) {
        if (typeof input === 'string') {
            input = offsetFromString(matchShortOffset, input);
            if (input === null) {
                return this;
            }
        } else if (Math.abs(input) < 16 && !keepMinutes) {
            input = input * 60;
        }
        if (!this._isUTC && keepLocalTime) {
            localAdjust = getDateOffset(this);
        }
        this._offset = input;
        this._isUTC = true;
        if (localAdjust != null) {
            this.add(localAdjust, 'm');
        }
        if (offset !== input) {
            if (!keepLocalTime || this._changeInProgress) {
                addSubtract(this, createDuration(input - offset, 'm'), 1, false);
            } else if (!this._changeInProgress) {
                this._changeInProgress = true;
                hooks.updateOffset(this, true);
                this._changeInProgress = null;
            }
        }
        return this;
    } else {
        return this._isUTC ? offset : getDateOffset(this);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.valueOf"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>valueOf ()](#apidoc.element.moment-timezone.fn.valueOf)
- description and source-code
```javascript
function valueOf() {
    return this._d.valueOf() - ((this._offset || 0) * 60000);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.week"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>week (input)](#apidoc.element.moment-timezone.fn.week)
- description and source-code
```javascript
function getSetWeek(input) {
    var week = this.localeData().week(this);
    return input == null ? week : this.add((input - week) * 7, 'd');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.weekYear"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>weekYear (input)](#apidoc.element.moment-timezone.fn.weekYear)
- description and source-code
```javascript
function getSetWeekYear(input) {
    return getSetWeekYearHelper.call(this,
            input,
            this.week(),
            this.weekday(),
            this.localeData()._week.dow,
            this.localeData()._week.doy);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.weekday"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>weekday (input)](#apidoc.element.moment-timezone.fn.weekday)
- description and source-code
```javascript
function getSetLocaleDayOfWeek(input) {
    if (!this.isValid()) {
        return input != null ? this : NaN;
    }
    var weekday = (this.day() + 7 - this.localeData()._week.dow) % 7;
    return input == null ? weekday : this.add(input - weekday, 'd');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.weeks"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>weeks (input)](#apidoc.element.moment-timezone.fn.weeks)
- description and source-code
```javascript
function getSetWeek(input) {
    var week = this.localeData().week(this);
    return input == null ? week : this.add((input - week) * 7, 'd');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.weeksInYear"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>weeksInYear ()](#apidoc.element.moment-timezone.fn.weeksInYear)
- description and source-code
```javascript
function getWeeksInYear() {
    var weekInfo = this.localeData()._week;
    return weeksInYear(this.year(), weekInfo.dow, weekInfo.doy);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.year"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>year (value)](#apidoc.element.moment-timezone.fn.year)
- description and source-code
```javascript
year = function (value) {
    if (value != null) {
        set$1(this, unit, value);
        hooks.updateOffset(this, keepTime);
        return this;
    } else {
        return get(this, unit);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.years"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>years ()](#apidoc.element.moment-timezone.fn.years)
- description and source-code
```javascript
years = function () {
    if (hooks.deprecationHandler != null) {
        hooks.deprecationHandler(null, msg);
    }
    if (firstTime) {
        var args = [];
        var arg;
        for (var i = 0; i < arguments.length; i++) {
            arg = '';
            if (typeof arguments[i] === 'object') {
                arg += '\n[' + i + '] ';
                for (var key in arguments[0]) {
                    arg += key + ': ' + arguments[0][key] + ', ';
                }
                arg = arg.slice(0, -2); // Remove trailing comma and space
            } else {
                arg = arguments[i];
            }
            args.push(arg);
        }
        warn(msg + '\nArguments: ' + Array.prototype.slice.call(args).join('') + '\n' + (new Error()).stack);
        firstTime = false;
    }
    return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.zone"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>zone ()](#apidoc.element.moment-timezone.fn.zone)
- description and source-code
```javascript
zone = function () {
    if (hooks.deprecationHandler != null) {
        hooks.deprecationHandler(null, msg);
    }
    if (firstTime) {
        var args = [];
        var arg;
        for (var i = 0; i < arguments.length; i++) {
            arg = '';
            if (typeof arguments[i] === 'object') {
                arg += '\n[' + i + '] ';
                for (var key in arguments[0]) {
                    arg += key + ': ' + arguments[0][key] + ', ';
                }
                arg = arg.slice(0, -2); // Remove trailing comma and space
            } else {
                arg = arguments[i];
            }
            args.push(arg);
        }
        warn(msg + '\nArguments: ' + Array.prototype.slice.call(args).join('') + '\n' + (new Error()).stack);
        firstTime = false;
    }
    return fn.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.zoneAbbr"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>zoneAbbr ()](#apidoc.element.moment-timezone.fn.zoneAbbr)
- description and source-code
```javascript
zoneAbbr = function () {
			if (this._z) { return this._z.abbr(this); }
			return old.call(this);
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.fn.zoneName"></a>[function <span class="apidocSignatureSpan">moment-timezone.fn.</span>zoneName ()](#apidoc.element.moment-timezone.fn.zoneName)
- description and source-code
```javascript
zoneName = function () {
			if (this._z) { return this._z.abbr(this); }
			return old.call(this);
		}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.moment-timezone.tz"></a>[module moment-timezone.tz](#apidoc.module.moment-timezone.tz)

#### <a name="apidoc.element.moment-timezone.tz.tz"></a>[function <span class="apidocSignatureSpan">moment-timezone.</span>tz (input)](#apidoc.element.moment-timezone.tz.tz)
- description and source-code
```javascript
function tz(input) {
		var args = Array.prototype.slice.call(arguments, 0, -1),
			name = arguments[arguments.length - 1],
			zone = getZone(name),
			out  = moment.utc.apply(null, args);

		if (zone && !moment.isMoment(input) && needsOffset(out)) {
			out.add(zone.parse(out), 'minutes');
		}

		out.tz(name);

		return out;
	}
```
- example usage
```shell
...

[![NPM version][npm-version-image]][npm-url] [![NPM downloads][npm-downloads-image]][npm-url] [![MIT License][license-image]][license
-url] [![Build Status][travis-image]][travis-url]

IANA Time Zone Database + [Moment.js](http://momentjs.com).

'''js
var june = moment("2014-06-01T12:00:00Z");
june.tz('America/Los_Angeles').format('ha z'); // 5am PDT
june.tz('America/New_York').format('ha z');    // 8am EDT
june.tz('Asia/Tokyo').format('ha z');          // 9pm JST
june.tz('Australia/Sydney').format('ha z');    // 10pm EST

var dec = moment("2014-12-01T12:00:00Z");
dec.tz('America/Los_Angeles').format('ha z');  // 4am PST
dec.tz('America/New_York').format('ha z');     // 7am EST
...
```

#### <a name="apidoc.element.moment-timezone.tz.Zone"></a>[function <span class="apidocSignatureSpan">moment-timezone.tz.</span>Zone (packedString)](#apidoc.element.moment-timezone.tz.Zone)
- description and source-code
```javascript
function Zone(packedString) {
		if (packedString) {
			this._set(unpack(packedString));
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.tz.add"></a>[function <span class="apidocSignatureSpan">moment-timezone.tz.</span>add (packed)](#apidoc.element.moment-timezone.tz.add)
- description and source-code
```javascript
function addZone(packed) {
		var i, name, split, normalized;

		if (typeof packed === "string") {
			packed = [packed];
		}

		for (i = 0; i < packed.length; i++) {
			split = packed[i].split('|');
			name = split[0];
			normalized = normalizeName(name);
			zones[normalized] = packed[i];
			names[normalized] = name;
			if (split[5]) {
				addToGuesses(normalized, split[2].split(' '));
			}
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.tz.guess"></a>[function <span class="apidocSignatureSpan">moment-timezone.tz.</span>guess (ignoreCache)](#apidoc.element.moment-timezone.tz.guess)
- description and source-code
```javascript
function guess(ignoreCache) {
		if (!cachedGuess || ignoreCache) {
			cachedGuess = rebuildGuess();
		}
		return cachedGuess;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.tz.link"></a>[function <span class="apidocSignatureSpan">moment-timezone.tz.</span>link (aliases)](#apidoc.element.moment-timezone.tz.link)
- description and source-code
```javascript
function addLink(aliases) {
		var i, alias, normal0, normal1;

		if (typeof aliases === "string") {
			aliases = [aliases];
		}

		for (i = 0; i < aliases.length; i++) {
			alias = aliases[i].split('|');

			normal0 = normalizeName(alias[0]);
			normal1 = normalizeName(alias[1]);

			links[normal0] = normal1;
			names[normal0] = alias[0];

			links[normal1] = normal0;
			names[normal1] = alias[1];
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.tz.load"></a>[function <span class="apidocSignatureSpan">moment-timezone.tz.</span>load (data)](#apidoc.element.moment-timezone.tz.load)
- description and source-code
```javascript
function loadData(data) {
		addZone(data.zones);
		addLink(data.links);
		tz.dataVersion = data.version;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.tz.names"></a>[function <span class="apidocSignatureSpan">moment-timezone.tz.</span>names ()](#apidoc.element.moment-timezone.tz.names)
- description and source-code
```javascript
function getNames() {
		var i, out = [];

		for (i in names) {
			if (names.hasOwnProperty(i) && (zones[i] || zones[links[i]]) && names[i]) {
				out.push(names[i]);
			}
		}

		return out.sort();
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.tz.needsOffset"></a>[function <span class="apidocSignatureSpan">moment-timezone.tz.</span>needsOffset (m)](#apidoc.element.moment-timezone.tz.needsOffset)
- description and source-code
```javascript
function needsOffset(m) {
		return !!(m._a && (m._tzm === undefined));
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.tz.setDefault"></a>[function <span class="apidocSignatureSpan">moment-timezone.tz.</span>setDefault (name)](#apidoc.element.moment-timezone.tz.setDefault)
- description and source-code
```javascript
setDefault = function (name) {
		if (major < 2 || (major === 2 && minor < 9)) {
			logError('Moment Timezone setDefault() requires Moment.js >= 2.9.0. You are using Moment.js ' + moment.version + '.');
		}
		moment.defaultZone = name ? getZone(name) : null;
		return moment;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.tz.unpack"></a>[function <span class="apidocSignatureSpan">moment-timezone.tz.</span>unpack (string)](#apidoc.element.moment-timezone.tz.unpack)
- description and source-code
```javascript
function unpack(string) {
		var data = string.split('|'),
			offsets = data[2].split(' '),
			indices = data[3].split(''),
			untils  = data[4].split(' ');

		arrayToInt(offsets);
		arrayToInt(indices);
		arrayToInt(untils);

		intToUntil(untils, indices.length);

		return {
			name       : data[0],
			abbrs      : mapIndices(data[1].split(' '), indices),
			offsets    : mapIndices(offsets, indices),
			untils     : untils,
			population : data[5] | 0
		};
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.tz.unpackBase60"></a>[function <span class="apidocSignatureSpan">moment-timezone.tz.</span>unpackBase60 (string)](#apidoc.element.moment-timezone.tz.unpackBase60)
- description and source-code
```javascript
function unpackBase60(string) {
		var i = 0,
			parts = string.split('.'),
			whole = parts[0],
			fractional = parts[1] || '',
			multiplier = 1,
			num,
			out = 0,
			sign = 1;

		// handle negative numbers
		if (string.charCodeAt(0) === 45) {
			i = 1;
			sign = -1;
		}

		// handle digits before the decimal
		for (i; i < whole.length; i++) {
			num = charCodeToInt(whole.charCodeAt(i));
			out = 60 * out + num;
		}

		// handle digits after the decimal
		for (i = 0; i < fractional.length; i++) {
			multiplier = multiplier / 60;
			num = charCodeToInt(fractional.charCodeAt(i));
			out += num * multiplier;
		}

		return out * sign;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.tz.zone"></a>[function <span class="apidocSignatureSpan">moment-timezone.tz.</span>zone (name, caller)](#apidoc.element.moment-timezone.tz.zone)
- description and source-code
```javascript
function getZone(name, caller) {
		name = normalizeName(name);

		var zone = zones[name];
		var link;

		if (zone instanceof Zone) {
			return zone;
		}

		if (typeof zone === 'string') {
			zone = new Zone(zone);
			zones[name] = zone;
			return zone;
		}

		// Pass getZone to prevent recursion more than 1 level deep
		if (links[name] && caller !== getZone && (link = getZone(links[name], getZone))) {
			zone = zones[name] = new Zone();
			zone._set(link);
			zone.name = names[name];
			return zone;
		}

		return null;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.tz.zoneExists"></a>[function <span class="apidocSignatureSpan">moment-timezone.tz.</span>zoneExists (name)](#apidoc.element.moment-timezone.tz.zoneExists)
- description and source-code
```javascript
function zoneExists(name) {
		if (!zoneExists.didShowError) {
			zoneExists.didShowError = true;
				logError("moment.tz.zoneExists('" + name + "') has been deprecated in favor of !moment.tz.zone('" + name + "')");
		}
		return !!getZone(name);
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.moment-timezone.tz.Zone"></a>[module moment-timezone.tz.Zone](#apidoc.module.moment-timezone.tz.Zone)

#### <a name="apidoc.element.moment-timezone.tz.Zone.Zone"></a>[function <span class="apidocSignatureSpan">moment-timezone.tz.</span>Zone (packedString)](#apidoc.element.moment-timezone.tz.Zone.Zone)
- description and source-code
```javascript
function Zone(packedString) {
		if (packedString) {
			this._set(unpack(packedString));
		}
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.moment-timezone.tz.Zone.prototype"></a>[module moment-timezone.tz.Zone.prototype](#apidoc.module.moment-timezone.tz.Zone.prototype)

#### <a name="apidoc.element.moment-timezone.tz.Zone.prototype._index"></a>[function <span class="apidocSignatureSpan">moment-timezone.tz.Zone.prototype.</span>_index (timestamp)](#apidoc.element.moment-timezone.tz.Zone.prototype._index)
- description and source-code
```javascript
_index = function (timestamp) {
			var target = +timestamp,
				untils = this.untils,
				i;

			for (i = 0; i < untils.length; i++) {
				if (target < untils[i]) {
					return i;
				}
			}
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.tz.Zone.prototype._set"></a>[function <span class="apidocSignatureSpan">moment-timezone.tz.Zone.prototype.</span>_set (unpacked)](#apidoc.element.moment-timezone.tz.Zone.prototype._set)
- description and source-code
```javascript
_set = function (unpacked) {
			this.name       = unpacked.name;
			this.abbrs      = unpacked.abbrs;
			this.untils     = unpacked.untils;
			this.offsets    = unpacked.offsets;
			this.population = unpacked.population;
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.tz.Zone.prototype.abbr"></a>[function <span class="apidocSignatureSpan">moment-timezone.tz.Zone.prototype.</span>abbr (mom)](#apidoc.element.moment-timezone.tz.Zone.prototype.abbr)
- description and source-code
```javascript
abbr = function (mom) {
			return this.abbrs[this._index(mom)];
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.tz.Zone.prototype.offset"></a>[function <span class="apidocSignatureSpan">moment-timezone.tz.Zone.prototype.</span>offset (mom)](#apidoc.element.moment-timezone.tz.Zone.prototype.offset)
- description and source-code
```javascript
offset = function (mom) {
			return this.offsets[this._index(mom)];
		}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.moment-timezone.tz.Zone.prototype.parse"></a>[function <span class="apidocSignatureSpan">moment-timezone.tz.Zone.prototype.</span>parse (timestamp)](#apidoc.element.moment-timezone.tz.Zone.prototype.parse)
- description and source-code
```javascript
parse = function (timestamp) {
			var target  = +timestamp,
				offsets = this.offsets,
				untils  = this.untils,
				max     = untils.length - 1,
				offset, offsetNext, offsetPrev, i;

			for (i = 0; i < max; i++) {
				offset     = offsets[i];
				offsetNext = offsets[i + 1];
				offsetPrev = offsets[i ? i - 1 : i];

				if (offset < offsetNext && tz.moveAmbiguousForward) {
					offset = offsetNext;
				} else if (offset > offsetPrev && tz.moveInvalidForward) {
					offset = offsetPrev;
				}

				if (target < untils[i] - (offset * 60000)) {
					return offsets[i];
				}
			}

			return offsets[max];
		}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
