^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package catkin_simple
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

0.2.0 (2018-10-18)
------------------
* Merge pull request `#27 <https://github.com/catkin/catkin_simple/issues/27>`_ from flaviofontana/patch-1
  add dynamic reconfigure info to the readme
* add dynamic reconfigure info to the readme
* Merge pull request `#26 <https://github.com/catkin/catkin_simple/issues/26>`_ from flaviofontana/add_dynamic_reconfigure
  added autodetection of dynamic_reconfigure
* fixed indentation
* adding build dependency on gencfg
* adding all cfg all files at once
* added autodetection of dynamic_reconfigure
* Merge pull request `#25 <https://github.com/catkin/catkin_simple/issues/25>`_ from simonlynen/patch-1
  Fix typo
* Update catkin_simple-extras.cmake.em
* only install Media, not media, automatically
* [style] remove trailing whitespace
* Merge branch 'feature/install_roslaunch_files' of https://github.com/ethz-asl/catkin_simple into ethz-asl-feature/install_roslaunch_files
* Add informative cs_install() cmake output.
* cs_install() installs shared content folders
  * launch, rviz, urdf, meshes, maps, worlds, media and param
* Added automatic installation of roslaunch files with cs_install() macro if a launch folder exists in the source directory
* Merge pull request `#22 <https://github.com/catkin/catkin_simple/issues/22>`_ from ethz-asl/fix/install-include
  Fixed a bug in the install target for include directories
* Merge pull request `#2 <https://github.com/catkin/catkin_simple/issues/2>`_ from ethz-asl/fix/install-include
  Fix/install include
* Fixed a bug in the install target for include directories
* Merge pull request `#1 <https://github.com/catkin/catkin_simple/issues/1>`_ from catkin/master
  Pulling in changes from catkin
* Contributors: Flavio Fontana, Paul Furgale, Simon Lynen, Ulrich Schwesinger, William Woodall

0.1.1 (2014-09-16)
------------------
* Merge pull request `#20 <https://github.com/catkin/catkin_simple/issues/20>`_ from ethz-asl/feature/require_all_dependencies
  Updated the documentation to describe the feature.
* Updated the documentation to describe the feature
* Merge pull request `#19 <https://github.com/catkin/catkin_simple/issues/19>`_ from ethz-asl/feature/require_all_dependencies
  Added a feature to require all dependencies when calling find_package()
* Addressed comments
* Added a feature to require all dependencies when calling find_package()
* Merge pull request `#16 <https://github.com/catkin/catkin_simple/issues/16>`_ from simonlynen/fix/readme_python_script_example
  Update Readme.md to call cs_install_scripts.
* Update Readme.md to call cs_install_scripts.
* Merge pull request `#15 <https://github.com/catkin/catkin_simple/issues/15>`_ from rhololkeolke/master
  Added autogeneration of actions. Fixes `#5 <https://github.com/catkin/catkin_simple/issues/5>`_
* Added autogeneration of actions. Fixes `#5 <https://github.com/catkin/catkin_simple/issues/5>`_
* add NO_AUTO_LINK, NO_AUTO_DEP, and NO_AUTO_EXPORT
  These apply to the cs_add_executable and
  cs_add_library macros. The NO_AUTO_LINK does not
  link against catkin_LIBRARIES automatically. The
  NO_AUTO_DEP option does not automatically depend
  on catkin_EXPORTED_TARGETS, and the NO_AUTO_EXPORT
  only applies to libraries and does not
  automatically export a library into cs_export and
  therefore not into catkin_package.
* Merge pull request `#13 <https://github.com/catkin/catkin_simple/issues/13>`_ from catkin/change_pkg_target_name
  Avoid non-obvious target name rewritting
* change failure style on colliding target names
  also changed the cs_add_target_to_package to be
  cs_add_targets_to_package which can take multiple
  targets
* use ${PROJECT_NAME}_package as the top-level target for a package
  this means no more renaming of execs and libs
* Merge pull request `#12 <https://github.com/catkin/catkin_simple/issues/12>`_ from catkin/cs_add_library_fix
  fix issue with propagating wrong library name, unroll recursion
* fix issue with propagating wrong library name, unroll recursion
* Merge pull request `#11 <https://github.com/catkin/catkin_simple/issues/11>`_ from tfoote/patch-1
  fix copy and paste error _lib vs _exec
* fix copy and paste error _lib vs _exec
  In add library it was adding properties to _exec instead of _lib
* Merge pull request `#9 <https://github.com/catkin/catkin_simple/issues/9>`_ from dirk-thomas/patch-1
  propagate catkin dependency downstream
* propagate catkin dependency downstream
* Merge pull request `#8 <https://github.com/catkin/catkin_simple/issues/8>`_ from catkin/project_level_target
  add project target for each catkin_simple package
* fix target name collision handling for execs/libs
* add project target for each catkin_simple package
  If an executable or library with the same name is
  added using cs\_ prefixed macros then they will be
  automatically renamed to ${PROJECT_NAME}_exec and
  ${PROJECT_NAME}_lib respectively.
* add Dirk as an author/maintainer
* Update README.md
* More readme updates
* Merge branch 'master' of https://github.com/wjwwood/catkin_simple
  Conflicts:
  README.rst
* Change readme to markdown for syntax highlighting
* Merge pull request `#4 <https://github.com/catkin/catkin_simple/issues/4>`_ from dirk-thomas/master
  add message generation if necessary
* add message generation if necessary
* Merge pull request `#2 <https://github.com/catkin/catkin_simple/issues/2>`_ from dirk-thomas/master
  fix add_dependencies for empty export targets
* fix add_dependencies for empty export targets
* Merge pull request `#1 <https://github.com/catkin/catkin_simple/issues/1>`_ from dirk-thomas/master
  some fixes and enhancements
* passing run_depends (instead of build_depends) as CATKIN_DEPENDS to cs_export
* fix passing DEPENDS to cs_export
* prevent install files from .svn subfolders
* add dependency on catkin_EXPORTED_TARGETS for executables and libraries
* allow passing multiple scripts to cs_install_scripts
* Removed any reference to <depend> tag, leave that for a different experiment
* more readme
* Added a readme
* relocating tests
* Fixing problem when include directory does not exist
* Merge branch 'no_catkin_depend'
  Conflicts:
  cmake/catkin_simple-extras.cmake.em
* Looks like this is not going to work
* Added cs_install macros
* Added cs_install macros
* cleanup of dead code
* Working without catkin_depends
* Improving tests
* Initial catkin_simple implementation (with catkin_depend tag).
* Contributors: Devin Schwab, Dirk Thomas, Paul Furgale, Simon Lynen, Tully Foote, William Woodall
