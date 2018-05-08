# Final Project Research Plan
&nbsp;
#### My Project idea
Creating a custom linux distrobution designed to monitor and diagnose hardware failures and suggest repairs or replacements
&nbsp;
#### Necessary Research
- Other Linux distros with a similar goal in mind
- A Linux distro to begin with which would then be customized to my needs
    - Or possibly LFS (linux from scratch)?
    - Tools to customize linux
    - Tools to repack OS as iso
- What tools are available for diagnosing hardware problems
    - Are some of those tools better than others?
    - Could I develop software to read HW error codes and recommend repairs
- Potential costs
    - Likely very little if any since most linux software is open source
        - Might need a flash drive

#### Potential Challenges
- Scope
    - Developing custom software to read error codes may be too intensive
    - LFS could be a lot of work, as well as installing arch from scratch
    - Effectively monitoring every part of hardware may be difficult
- Compatibility
    - Software compatibility with hardware varies greatly from computer to computer
    - The change from BIOS to UEFI for new computers may prove tricky to boot on older systems
    - Different hardware manufacturers have different drivers that all need to be installed and automatically turned on when detected
- Many programs for linux are deprecated or not updated very often meaning selection of diagnostic tools may be limited

#### Realistic Goal
Create a flashdrive with a full install of a linux distro that is at least stripped down and customized with tools for Monitoring and Diagnosing HW.
