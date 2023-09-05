# Compare the data masking component to the data masking plugin

The Data Masking component feature is in [tech preview](glossary.md#tech-preview).

Percona Server for MySQL 8.0.34 adds the data masking component. Either the component or the plugin extends the server's functionality, but the architecture of a plugin is different than the component. 

The main differences between the component and plugin are the following:

| Component | Plugin |
|--- | --- |
| Allows multi-byte character sets for the general-purpose masking functions | Does not allow multi-byte character sets |
| Supports masking PAN, SSN, IBAN, UUID, Canada SIN, and UK NIN | Supports masking PAN and SSN |
| Generates random email, US phone, PAN, SSN, IBAN, UUID, Canada SIN, and UK NIN data |  Generates random email, US phone, PAN, and SSN |
| Supports persisting substitution dictionaries in the database | Supports persisting substitution dictionaries in a file |
| Supports a dedicated privilege to manage the dictionaries | Requires a file privilege |

