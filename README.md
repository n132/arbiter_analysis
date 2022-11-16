# Issue: It's hard to debug 
- How to debug
  - Learn the installing
    - Use setuptools
  - The answer import local one rather than the one installed
    - Change the import setting to let it import local one
      - sys.path.append('/mnt/arbiter')
      - from arbiter.master_chief import *
  - Now we can change the code and debugging!

# 