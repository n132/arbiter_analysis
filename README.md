# Issue: It's hard to debug 
- How to debug
  - Learn the installing
    - Use setuptools
  - Answer
    - build + install again
    - Less painful with a script


# Issue: Add wrong targets during arbiter.master_chief.sa_recon

- Todo: case-> /bin/sh
  - python3 ./run_arbiter.py -f ./CWE131.py -t /bin/ls -l ./n132_log -j ./n132_json
  - 

# Issue: why the apply_constraint returns nothing [False Positive Issue]
- Constrain is applied to the state
- It's false postive 

# Issue: Why apply constrain to all init_val rather than related val


# Issue: Track right case
- checkpoit comes from souce: if there is no source for the vul, it should be {}
  - If it's {}, sa_advanced:analyze_one would set "target.source = target.addr"
  - in symbolic execution, call chain would be run_all->run_one->_execute_one-> _create_entry_state+_explore_one
- The issue's origin is in sa_advanced->_find_source. There is a KeyError.
- 