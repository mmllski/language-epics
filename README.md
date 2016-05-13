EPICS Database support in Atom
======

Add syntax highlighting and snippets to *.db files in Atom.

Preview
---

![demo](https://j.gifs.com/kRlojN.gif)

Installation
---

```sh
apm install language-epics
```

or find it in the Packages tab under Settings.

Available snippets
---
| Trigger       | Name                          | Body                                                                                              |
| ------------- |---------------------------    | --------------------------------------------------------------------------------------------------|
| record        | generic record                | record(record_type "record_name") { }                                                             |
| macro         | generic macro                 | $(MACRO)                                                                                          |
| field         | generic field                 | field(field_type,  "field_value")                                                                       |
| desc          | description field             | field(DESC,  "description")                                                                       |
| val          | value field                    | field(VAL,  "value")                                                                       |
| prec          | precision field               | field(PREC,  "precision")                                                                         |
| egu           | engineering units field       | field(EGU,  "unit")                                                                               |
| pini          | pini field                    | field(PINI,  "YESNO")                                                                             |
| fwd           | forward link field            | field(FLNK,  "record_name")                                                                       |
| scan          | scan field                    | field(SCAN,  ".1 second.2 second.5 second1 second2 second5 second10 secondI/O IntrEventPassive")  |
| inp           | input link field              | field(INP,  "record_name")                                                                        |
| out           | output link field             | field(OUT,  "record_name")                                                                        |
| dtyp          | device type field             | field(DTYP,  "Soft Channelstream")                                                                |
| dol           | desired output location field | field(DOL,  "record_name")                                                                        |
| selm          | selection mechanism field     | field(SELM,  "AllSpecifiedMask")                                                                  |
| omsl          | output mode select field      | field(OMSL,  "Supervisoryclosed_loop")                                                            |
| hihi          | hihi alarm limit field        | field(HIHI,  "float")                                                                             |
| high          | high alarm limit field        | field(HIGH,  "float")                                                                             |
| low           | low alarm limit field         | field(LOW,  "float")                                                                              |
| lolo          | lolo alarm limit field        | field(LOLO,  "float")                                                                             |
| hhsv          | hihi alarm severity field     | field(HHSV,  "NO_ALARMMINORMAJOR")                                                                |
| hsv           | high alarm severity field     | field(HSV,  "NO_ALARMMINORMAJOR")                                                                 |
| lsv           | low alarm severity field      | field(LSV,  "NO_ALARMMINORMAJOR")                                                                 |
| llsv          | lolo alarm severity field     | field(LLSV,  "NO_ALARMMINORMAJOR")                                                                |
| hyst          | alarm deadband field          | field(HYST,  "double")                                                                            |
| alarms        | all alarms fields             | insert fields: HIHI, HIGH, LOW,  LOLO, HHSV, HSV,  LSV,  LLSV, HYST                               |
| bi            | binary input record           | insert bi record with fields: DESC, VAL, ONAM, ZNAM                                               |
| bo            | binary output record          | insert bo record with fields: DESC, VAL, ONAM, ZNAM                                               |
| asub          | aSub record                   | insert aSub record with fields: DESC, SNAM, INPA, FTA, NOA, OUTA, FTVA, NOVA                      |
| calc          | calc record                   | insert calc record with fields: DESC, CALC, INPA, INPB                                            |
| calcout       | calcout record                | insert calcout record with fields: DESC, CALC, INPA, INPB, OUT                                    |
| dfanout       | dfanout record                | insert dfanout record with fields: DESC, OUTA, OUTB, DOL, OMSL                                    |
| fanout        | fanout record                 | insert fanout record with fields: DESC, SELM, SELN, SELL, LNKA, LNKB                              |
| sel           | select record                 | insert sel record with fields: DESC, SELM, SELN,  SELL, INPA, INPB, INPC                          |
| seq           | sequence record               | insert seq record with fields: DESC, SELM, SELN, SELL, DLY1, DOL1, LNK1, DLY2, DOL2, LNK2         |
| waveform      | waveform record               | insert waveform record with fields: DESC, NELM, FTVL                                              |



