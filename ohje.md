# Asenna KDiff3 Homebrew'n avulla

brew install kdiff3
brew info kdiff3

# Varmista, että Homebrew on päivitetty ennen asennusta:

brew update
brew upgrade

# Tarkista asennustiedot:

brew info kdiff3

# Konfiguroi Git KDiff3:lle

# Aseta diff-työkaluksi KDiff3:

git config --global diff.tool kdiff3
git config --global difftool.kdiff3.path "/opt/homebrew/Caskroom/kdiff3/1.11.0/kdiff3.wrapper.sh"
git config --global difftool.prompt false

# Aseta merge-työkaluksi KDiff3:

git config --global merge.tool kdiff3
git config --global mergetool.kdiff3.path "/opt/homebrew/Caskroom/kdiff3/1.11.0/kdiff3.wrapper.sh"
git config --global mergetool.prompt false

# Tarkista, että KDiff3 on asennettu ja toimii:

kdiff3 --version
