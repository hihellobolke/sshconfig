Dynamic sshconfig
====================

Sometime you want sshconfig different based on your target host, or your current OS or hostname. Here's a hacky convoluted script that I wrote. It eases my pain, I hope it gives you ideas if you're looking for some.


### Install Instructions

  - Download it and save in ~/bin
  - echo 'export PATH=~/bin:$PATH' >> ~/.bashrc
  - source ~/.bashrc
  
```
  
  # download ssh in your ~/bin
  ( mkdir ~/bin 2>/dev/null;
    cd ~/bin && wget -o ssh https://raw.github.com/hihellobolke/sshconfig/master/ssh && chmod 755 ssh
  )


  # add ~/bin to PATH in your ~/.bashrc
  echo 'export PATH=~/bin:$PATH' >> ~/.bashrc
  source ~/.bashrc

```
