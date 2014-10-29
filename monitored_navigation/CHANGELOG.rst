^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package monitored_navigation
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

0.0.1 (2014-10-29)
------------------
* correcting help manager include
* Merge branch 'hydro-devel' of https://github.com/strands-project/strands_navigation into hydro-devel
  Conflicts:
  message_store_map_switcher/CMakeLists.txt
* making monitored_navigation a general smach based repo that allows user to add specific instantiations of smach monitors and smach recovery behaviours
* Adding Missing TopologicalMap.msg and changing maintainer emails, names and Licences for Packages
* changing param defauls;
  aborting when continuous nav action server does not exist
* taking out distinction between local and global plan failure
  first steps to make monitored_nav scitos independent
  always oututs after help
  new action definition
  less management of new goals arriving during execution, as it was buggy
* Renamed ros_datacentre to mongodb_store
  This simply bulk replaces all ros_datacentre strings to mongodb_store strings inside files and also in file names.
  Needs `strands-project/ros_datacentre#76 <https://github.com/strands-project/ros_datacentre/issues/76>`_ to be merged first.
* changing server nave for instrospection
* adding introspection seerver to monitored_navigation
* alternative preemption
* stopped preempting monitored_nav action when help is being offered by human. more edits for proper preemption of continuous nav action
* waiting more time to timeout previous action
* missing logging component
* add logging and making preemption work after recovery
* improving preemption mechanism
* bug fix
* goals are only replaced when the new goal has the same action server name
* sovling time/duration comparisons bug
* disabling backtrack for now
* Adding machine tags to launch files
* Merge branch 'hydro-devel' of https://github.com/BFALacerda/strands_navigation into hydro-devel
* small bug fixes
* monitored navigation now does not cancel move_base when new goal arrives
* use ptu action from scitos_ptu
* Checking for preemption and added a few dependencies for recover states
* monitored navigation now does not ask for help when NavFn fails, as it usually means that the goal pose is blocked by an obstacle
* Added backwards driving behaviour
* adding state to be filled with moving backwards recovery
* - ability to preempt bumper recovery
  - send interaction_service without the prefix
* removed scitos_2d_nav of monitored_nav.launch
* added monitored navigation gui
* code cleaning
* getting preemption to work properly
* making the continuous navigation action server an input to the monitored navigation
* code cleaning
* making human help optional
* adding manager node for human help interfaces - first version
* first version of monitored navigation
* Contributors: BFALacerda, Bob, Bruno Lacerda, Chris Burbridge, Jaime Pulido Fentanes, Lars Kunze, Nick Hawes, Nils Bore, strands