# Device Data Formatting
Docuconsult File Format proposal

# Todo
- [x] Create first basis for the format proposal
- [ ] Incorporate realistic fields from a real Usage Report
- [ ] Get manufacturer cooperation
- [ ] Process internal feedback
- [ ] Process manufacturer feedback
- [ ] Write validator script
- [ ] Write importer

# Device Export File
The file devices-example.json shows some example data of a devic export. The following details are important to note.
- SerialNumber, Manufacturer and DeviceType are required, other fields are optional
- Dates are UTC formatted strings
- SerialNumber values are strings and must be unique as they are used as unique identifiers

# Usage Report File
The file usage-example.json shows some example data of a usage report. The following details are important to note.
- Dates are again UTC formatted strings. ExportDateUTC is the moment the data is exported whereas PeriodStartUTC and PeriodEndUTC indicate the period contained in the log.
- PrintVolume is an integer indicating the amount of pages printed in this period by this device.
