## Storage

- Verify that all drives show up. The R550 has a bad backplane design which may cause some pins on the HBA to not come in contact with the backplane. Reseating the backplane and reconnecting the HBA may help.
- iDRAC will only show 1 drive per PCIe device attached. For example, with the Intel DC P4608 drive which is actually 2 drives on a single PCIe card, only 1 drive will show up.