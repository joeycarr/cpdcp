# cpdcp
Copy Digital Cinema Packages (DCPs) onto disk for distribution and format the disk appropriately.

    usage: cpdcp dcp_directory device

    Formats a destination volume as ext2 with appropriate permissions,
    inode size, and zero reserved space. This is useful for putting DCPs
    onto flash drives. For maximum compatibility the drive should have a
    single partition with a Master Boot Record partition scheme (the
    default for most flash drives).

    positional arguments:
    dcp_directory   This directory should contain your DCP's
                    VOLINDEX.xml file.
    device          This should be a block device, e.g. a USB drive.

Implemented as a bash script, this program is a bespoke workflow aid
in the production and distribution of DCPs. I collected a lot of
advice on compatibility from teh interwebs and we have screened many
short films without failure. The script has been used with Ubuntu
Server 14.04.1, running under VirtualBox, hosted on a Mac Pro.
