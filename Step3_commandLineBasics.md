## Basic commands

1. List the contents of the current directory
```bash
ls
```

2. Display the current directory path
```bash
pwd
```

3. Change to a different directory and check if the current directory has been changed
```bash
cd ~
pwd
```

4. Check if you have **wget** and install if necessary

Mac
```bash
# Check if wget is installed
wget --version

# If wget is not installed, check if homebrew is installed
brew --version

# If brew is not installed, install it:
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# Install wget using brew
brew install wget

# Confirm that it worked
wget --version
```
[Mac instructions](https://www.jcchouinard.com/wget/#Download_Wget_on_Mac)

Linux/Ubuntu
```bash
# See if wget is installed
wget --version

# Install 
apt-get install wget

# Confirm that it worked
wget --version
```
[Linux instructions](https://www.tecmint.com/install-wget-in-linux/)

Windows users: Follow Ubuntu instructions above if you have installed Ubuntu
[Windows instructions](https://www.jcchouinard.com/wget/#Download_Wget_on_Windows)

5. Try downloading an external file
```bash
wget https://adimitromanolakis.github.io/truffle/fs-and-po-pairs-from-1000genomes.vcf.gz
```

6. Find the file size of fs-and-po-pairs-from-1000genomes.vcf by running 
```bash
ls -hl
```

7. Unzip the .gz file (depends on Operating System)
```bash
gunzip fs-and-po-pairs-from-1000genomes.vcf.gz
```

8. Print the last ten lines of the .vcf file
```bash
tail -n 10 fs-and-po-pairs-from-1000genomes.vcf
```

9. Find the number of lines in .vcf file fs-and-po-pairs-from-1000genomes.vcf
```bash
wc -l fs-and-po-pairs-from-1000genomes.vcf
```

10. Create your own directory
```bash
mkdir variants
ls -hl
```

11. Copy a file
```bash
cp fs-and-po-pairs-from-1000genomes.vcf testcopy.vcf
ls -hl
```

12. Move a file to another directory
```bash
mv testcopy.vcf variants
ls -hl
ls -hl variants
```