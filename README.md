# error_log
an error log for installing CommonRoad on Windows 10

Steps taken:
[1] create a new environment in my Anaconda Navigator called `cmRd` with Python 3.8.13;
[1] within the `cmRd` environment, in a windows command window, use 
```
pip install commonroad-io commonroad-drivability-checker
```
This is where the problem occurred. The installation did not complete but produced errors. The log from the windows command window is the following (it is kind of long):

```
(cmRd) C:\Users\Tong>pip install commonroad-io commonroad-drivability-checker
Collecting commonroad-io
  Downloading commonroad_io-2022.1-py3-none-any.whl (3.6 MB)
     |████████████████████████████████| 3.6 MB 1.1 MB/s
Collecting commonroad-drivability-checker
  Downloading commonroad-drivability-checker-2021.4.1.tar.gz (9.9 MB)
     |████████████████████████████████| 9.9 MB 939 kB/s
Collecting scipy>=1.5.2
  Downloading scipy-1.8.0-cp38-cp38-win_amd64.whl (36.9 MB)
     |████████████████████████████████| 36.9 MB 599 kB/s
Collecting commonroad-vehicle-models>=2.0.0
  Using cached commonroad_vehicle_models-2.0.0-py3-none-any.whl (37 kB)
Collecting lxml>=4.2.2
  Downloading lxml-4.8.0-cp38-cp38-win_amd64.whl (3.6 MB)
     |████████████████████████████████| 3.6 MB 1.1 MB/s
Collecting shapely>=1.6.4
  Downloading Shapely-1.8.1.post1-cp38-cp38-win_amd64.whl (1.3 MB)
     |████████████████████████████████| 1.3 MB 1.1 MB/s
Collecting rtree>=0.8.3
  Downloading Rtree-1.0.0-cp38-cp38-win_amd64.whl (433 kB)
     |████████████████████████████████| 433 kB 1.1 MB/s
Collecting iso3166>=1.0.1
  Using cached iso3166-2.0.2-py3-none-any.whl (8.5 kB)
Collecting networkx>=2.2
  Downloading networkx-2.8-py3-none-any.whl (2.0 MB)
     |████████████████████████████████| 2.0 MB 930 kB/s
Collecting Pillow>=7.0.0
  Downloading Pillow-9.1.0-cp38-cp38-win_amd64.whl (3.3 MB)
     |████████████████████████████████| 3.3 MB 930 kB/s
Collecting matplotlib>=3.0.0
  Downloading matplotlib-3.5.1-cp38-cp38-win_amd64.whl (7.2 MB)
     |████████████████████████████████| 7.2 MB 1.1 MB/s
Collecting numpy>=1.13
  Downloading numpy-1.22.3-cp38-cp38-win_amd64.whl (14.7 MB)
     |████████████████████████████████| 14.7 MB 731 kB/s
Collecting polygon3>=3.0.8
  Downloading Polygon3-3.0.9.1.tar.gz (39 kB)
Collecting triangle>=20200424
  Downloading triangle-20220202-cp38-cp38-win_amd64.whl (1.4 MB)
     |████████████████████████████████| 1.4 MB 1.3 MB/s
Collecting python-dateutil>=2.7
  Downloading python_dateutil-2.8.2-py2.py3-none-any.whl (247 kB)
     |████████████████████████████████| 247 kB 1.1 MB/s
Collecting cycler>=0.10
  Downloading cycler-0.11.0-py3-none-any.whl (6.4 kB)
Collecting fonttools>=4.22.0
  Downloading fonttools-4.32.0-py3-none-any.whl (900 kB)
     |████████████████████████████████| 900 kB 939 kB/s
Collecting kiwisolver>=1.0.1
  Downloading kiwisolver-1.4.2-cp38-cp38-win_amd64.whl (55 kB)
     |████████████████████████████████| 55 kB 734 kB/s
Collecting packaging>=20.0
  Downloading packaging-21.3-py3-none-any.whl (40 kB)
     |████████████████████████████████| 40 kB 1.3 MB/s
Collecting pyparsing>=2.2.1
  Downloading pyparsing-3.0.7-py3-none-any.whl (98 kB)
     |████████████████████████████████| 98 kB 1.3 MB/s
Collecting six>=1.5
  Downloading six-1.16.0-py2.py3-none-any.whl (11 kB)
Building wheels for collected packages: commonroad-drivability-checker, polygon3
  Building wheel for commonroad-drivability-checker (setup.py) ... error
  ERROR: Command errored out with exit status 1:
   command: 'C:\ProgramData\Anaconda3\envs\cmRd\python.exe' -u -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'C:\\Users\\Tong\\AppData\\Local\\Temp\\pip-install-jdzwspsk\\commonroad-drivability-checker_1f5efd72f4dd4e98b5d7dd24fdbc71f8\\setup.py'"'"'; __file__='"'"'C:\\Users\\Tong\\AppData\\Local\\Temp\\pip-install-jdzwspsk\\commonroad-drivability-checker_1f5efd72f4dd4e98b5d7dd24fdbc71f8\\setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' bdist_wheel -d 'C:\Users\Tong\AppData\Local\Temp\pip-wheel-bx87aoow'
       cwd: C:\Users\Tong\AppData\Local\Temp\pip-install-jdzwspsk\commonroad-drivability-checker_1f5efd72f4dd4e98b5d7dd24fdbc71f8\
  Complete output (111 lines):
  C:\ProgramData\Anaconda3\envs\cmRd\lib\site-packages\setuptools\dist.py:717: UserWarning: Usage of dash-separated 'description-file' will not be supported in future versions. Please use the underscore name 'description_file' instead
    warnings.warn(
  running bdist_wheel
  running build
  running build_py
  creating build
  creating build\lib.win-amd64-3.8
  creating build\lib.win-amd64-3.8\commonroad_dc
  copying commonroad_dc\__init__.py -> build\lib.win-amd64-3.8\commonroad_dc
  running egg_info
  writing commonroad_drivability_checker.egg-info\PKG-INFO
  writing dependency_links to commonroad_drivability_checker.egg-info\dependency_links.txt
  writing requirements to commonroad_drivability_checker.egg-info\requires.txt
  writing top-level names to commonroad_drivability_checker.egg-info\top_level.txt
  reading manifest file 'commonroad_drivability_checker.egg-info\SOURCES.txt'
  reading manifest template 'MANIFEST.in'
  adding license file 'LICENSE'
  writing manifest file 'commonroad_drivability_checker.egg-info\SOURCES.txt'
  creating build\lib.win-amd64-3.8\commonroad_dc\boundary
  copying commonroad_dc\boundary\__init__.py -> build\lib.win-amd64-3.8\commonroad_dc\boundary
  copying commonroad_dc\boundary\boundary.py -> build\lib.win-amd64-3.8\commonroad_dc\boundary
  copying commonroad_dc\boundary\construction.py -> build\lib.win-amd64-3.8\commonroad_dc\boundary
  copying commonroad_dc\boundary\lanelet_bounds.py -> build\lib.win-amd64-3.8\commonroad_dc\boundary
  copying commonroad_dc\boundary\rectangle_builder.py -> build\lib.win-amd64-3.8\commonroad_dc\boundary
  copying commonroad_dc\boundary\scenario_bounds.py -> build\lib.win-amd64-3.8\commonroad_dc\boundary
  copying commonroad_dc\boundary\triangle_builder.py -> build\lib.win-amd64-3.8\commonroad_dc\boundary
  creating build\lib.win-amd64-3.8\commonroad_dc\collision
  copying commonroad_dc\collision\__init__.py -> build\lib.win-amd64-3.8\commonroad_dc\collision
  creating build\lib.win-amd64-3.8\commonroad_dc\collision\collision_detection
  copying commonroad_dc\collision\collision_detection\__init__.py -> build\lib.win-amd64-3.8\commonroad_dc\collision\collision_detection
  copying commonroad_dc\collision\collision_detection\minkowski_sum.py -> build\lib.win-amd64-3.8\commonroad_dc\collision\collision_detection
  copying commonroad_dc\collision\collision_detection\pycrcc_collision_dispatch.py -> build\lib.win-amd64-3.8\commonroad_dc\collision\collision_detection
  copying commonroad_dc\collision\collision_detection\scenario.py -> build\lib.win-amd64-3.8\commonroad_dc\collision\collision_detection
  creating build\lib.win-amd64-3.8\commonroad_dc\collision\trajectory_queries
  copying commonroad_dc\collision\trajectory_queries\trajectory_queries.py -> build\lib.win-amd64-3.8\commonroad_dc\collision\trajectory_queries
  copying commonroad_dc\collision\trajectory_queries\trajectory_queries_specialized.py -> build\lib.win-amd64-3.8\commonroad_dc\collision\trajectory_queries
  creating build\lib.win-amd64-3.8\commonroad_dc\collision\visualization
  copying commonroad_dc\collision\visualization\__init__.py -> build\lib.win-amd64-3.8\commonroad_dc\collision\visualization
  copying commonroad_dc\collision\visualization\drawing.py -> build\lib.win-amd64-3.8\commonroad_dc\collision\visualization
  creating build\lib.win-amd64-3.8\commonroad_dc\costs
  copying commonroad_dc\costs\__init__.py -> build\lib.win-amd64-3.8\commonroad_dc\costs
  copying commonroad_dc\costs\evaluation.py -> build\lib.win-amd64-3.8\commonroad_dc\costs
  copying commonroad_dc\costs\partial_cost_functions.py -> build\lib.win-amd64-3.8\commonroad_dc\costs
  copying commonroad_dc\costs\route_matcher.py -> build\lib.win-amd64-3.8\commonroad_dc\costs
  creating build\lib.win-amd64-3.8\commonroad_dc\feasibility
  copying commonroad_dc\feasibility\__init__.py -> build\lib.win-amd64-3.8\commonroad_dc\feasibility
  copying commonroad_dc\feasibility\feasibility_checker.py -> build\lib.win-amd64-3.8\commonroad_dc\feasibility
  copying commonroad_dc\feasibility\solution_checker.py -> build\lib.win-amd64-3.8\commonroad_dc\feasibility
  copying commonroad_dc\feasibility\vehicle_dynamics.py -> build\lib.win-amd64-3.8\commonroad_dc\feasibility
  creating build\lib.win-amd64-3.8\commonroad_dc\geometry
  copying commonroad_dc\geometry\__init__.py -> build\lib.win-amd64-3.8\commonroad_dc\geometry
  copying commonroad_dc\geometry\geometry.py -> build\lib.win-amd64-3.8\commonroad_dc\geometry
  copying commonroad_dc\geometry\lanelet_ccosy.py -> build\lib.win-amd64-3.8\commonroad_dc\geometry
  copying commonroad_dc\geometry\util.py -> build\lib.win-amd64-3.8\commonroad_dc\geometry
  running build_ext
  -- Building for: Visual Studio 16 2019
  -- Selecting Windows SDK version 10.0.19041.0 to target Windows 10.0.19043.
  -- The C compiler identification is MSVC 19.29.30037.0
  -- The CXX compiler identification is MSVC 19.29.30037.0
  -- Detecting C compiler ABI info
  -- Detecting C compiler ABI info - done
  -- Check for working C compiler: C:/Program Files (x86)/Microsoft Visual Studio/2019/Community/VC/Tools/MSVC/14.29.30037/bin/Hostx64/x64/cl.exe - skipped
  -- Detecting C compile features
  -- Detecting C compile features - done
  -- Detecting CXX compiler ABI info
  -- Detecting CXX compiler ABI info - done
  -- Check for working CXX compiler: C:/Program Files (x86)/Microsoft Visual Studio/2019/Community/VC/Tools/MSVC/14.29.30037/bin/Hostx64/x64/cl.exe - skipped
  -- Detecting CXX compile features
  -- Detecting CXX compile features - done
  -- Configuring done
  -- Generating done
  -- Build files have been written to: C:/Users/Tong/AppData/Local/Temp/pip-install-jdzwspsk/commonroad-drivability-checker_1f5efd72f4dd4e98b5d7dd24fdbc71f8/build/temp.win-amd64-3.8/Release/build
  Microsoft (R) Build Engine version 16.10.1+2fd48ab73 for .NET Framework
  Copyright (C) Microsoft Corporation. All rights reserved.

  MSBUILD : error MSB1004: Specify the name of the target.
  Switch: --target

  For switch syntax, type "MSBuild -help"
  Traceback (most recent call last):
    File "<string>", line 1, in <module>
    File "C:\Users\Tong\AppData\Local\Temp\pip-install-jdzwspsk\commonroad-drivability-checker_1f5efd72f4dd4e98b5d7dd24fdbc71f8\setup.py", line 139, in <module>
      setup(
    File "C:\ProgramData\Anaconda3\envs\cmRd\lib\site-packages\setuptools\__init__.py", line 153, in setup
      return distutils.core.setup(**attrs)
    File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\core.py", line 148, in setup
      dist.run_commands()
    File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\dist.py", line 966, in run_commands
      self.run_command(cmd)
    File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\dist.py", line 985, in run_command
      cmd_obj.run()
    File "C:\ProgramData\Anaconda3\envs\cmRd\lib\site-packages\wheel\bdist_wheel.py", line 299, in run
      self.run_command('build')
    File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\cmd.py", line 313, in run_command
      self.distribution.run_command(command)
    File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\dist.py", line 985, in run_command
      cmd_obj.run()
    File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\command\build.py", line 135, in run
      self.run_command(cmd_name)
    File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\cmd.py", line 313, in run_command
      self.distribution.run_command(command)
    File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\dist.py", line 985, in run_command
      cmd_obj.run()
    File "C:\Users\Tong\AppData\Local\Temp\pip-install-jdzwspsk\commonroad-drivability-checker_1f5efd72f4dd4e98b5d7dd24fdbc71f8\setup.py", line 42, in run
      self.build_extension(ext)
    File "C:\Users\Tong\AppData\Local\Temp\pip-install-jdzwspsk\commonroad-drivability-checker_1f5efd72f4dd4e98b5d7dd24fdbc71f8\setup.py", line 118, in build_extension
      subprocess.check_call(['cmake', '--build', '.'] + build_args, cwd=build_dir)
    File "C:\ProgramData\Anaconda3\envs\cmRd\lib\subprocess.py", line 364, in check_call
      raise CalledProcessError(retcode, cmd)
  subprocess.CalledProcessError: Command '['cmake', '--build', '.', '--config', 'Release', '--', '/m', '--target', 'install']' returned non-zero exit status 1.
  ['-DADD_PYTHON_BINDINGS=TRUE', '-DADD_TESTS=OFF', '-DBUILD_DOC=OFF', '-DPYTHON_INCLUDE_DIR=C:\\ProgramData\\Anaconda3\\envs\\cmRd\\Include', '-DPYTHON_LIBRARY=', '-DPYTHON_EXECUTABLE=C:\\ProgramData\\Anaconda3\\envs\\cmRd\\python.exe']
  ----------------------------------------
  ERROR: Failed building wheel for commonroad-drivability-checker
  Running setup.py clean for commonroad-drivability-checker
  Building wheel for polygon3 (setup.py) ... done
  Created wheel for polygon3: filename=Polygon3-3.0.9.1-cp38-cp38-win_amd64.whl size=51106 sha256=7c846753e3b7f2fedae4a9dc45e594563fbc51e140e73bee0e2fe4e5bb3918b9
  Stored in directory: c:\users\tong\appdata\local\pip\cache\wheels\49\63\6e\fdc7a306f863a60035fa86b3b017b363fd15eadd5a89ae027d
Successfully built polygon3
Failed to build commonroad-drivability-checker
Installing collected packages: six, pyparsing, python-dateutil, Pillow, packaging, numpy, kiwisolver, fonttools, cycler, shapely, scipy, rtree, networkx, matplotlib, lxml, iso3166, commonroad-vehicle-models, triangle, polygon3, commonroad-io, commonroad-drivability-checker
    Running setup.py install for commonroad-drivability-checker ... error
    ERROR: Command errored out with exit status 1:
     command: 'C:\ProgramData\Anaconda3\envs\cmRd\python.exe' -u -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'C:\\Users\\Tong\\AppData\\Local\\Temp\\pip-install-jdzwspsk\\commonroad-drivability-checker_1f5efd72f4dd4e98b5d7dd24fdbc71f8\\setup.py'"'"'; __file__='"'"'C:\\Users\\Tong\\AppData\\Local\\Temp\\pip-install-jdzwspsk\\commonroad-drivability-checker_1f5efd72f4dd4e98b5d7dd24fdbc71f8\\setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' install --record 'C:\Users\Tong\AppData\Local\Temp\pip-record-levpxnqh\install-record.txt' --single-version-externally-managed --compile --install-headers 'C:\ProgramData\Anaconda3\envs\cmRd\Include\commonroad-drivability-checker'
         cwd: C:\Users\Tong\AppData\Local\Temp\pip-install-jdzwspsk\commonroad-drivability-checker_1f5efd72f4dd4e98b5d7dd24fdbc71f8\
    Complete output (113 lines):
    C:\ProgramData\Anaconda3\envs\cmRd\lib\site-packages\setuptools\dist.py:717: UserWarning: Usage of dash-separated 'description-file' will not be supported in future versions. Please use the underscore name 'description_file' instead
      warnings.warn(
    running install
    running build
    running build_py
    creating build
    creating build\lib.win-amd64-3.8
    creating build\lib.win-amd64-3.8\commonroad_dc
    copying commonroad_dc\__init__.py -> build\lib.win-amd64-3.8\commonroad_dc
    running egg_info
    writing commonroad_drivability_checker.egg-info\PKG-INFO
    writing dependency_links to commonroad_drivability_checker.egg-info\dependency_links.txt
    writing requirements to commonroad_drivability_checker.egg-info\requires.txt
    writing top-level names to commonroad_drivability_checker.egg-info\top_level.txt
    reading manifest file 'commonroad_drivability_checker.egg-info\SOURCES.txt'
    reading manifest template 'MANIFEST.in'
    adding license file 'LICENSE'
    writing manifest file 'commonroad_drivability_checker.egg-info\SOURCES.txt'
    creating build\lib.win-amd64-3.8\commonroad_dc\boundary
    copying commonroad_dc\boundary\__init__.py -> build\lib.win-amd64-3.8\commonroad_dc\boundary
    copying commonroad_dc\boundary\boundary.py -> build\lib.win-amd64-3.8\commonroad_dc\boundary
    copying commonroad_dc\boundary\construction.py -> build\lib.win-amd64-3.8\commonroad_dc\boundary
    copying commonroad_dc\boundary\lanelet_bounds.py -> build\lib.win-amd64-3.8\commonroad_dc\boundary
    copying commonroad_dc\boundary\rectangle_builder.py -> build\lib.win-amd64-3.8\commonroad_dc\boundary
    copying commonroad_dc\boundary\scenario_bounds.py -> build\lib.win-amd64-3.8\commonroad_dc\boundary
    copying commonroad_dc\boundary\triangle_builder.py -> build\lib.win-amd64-3.8\commonroad_dc\boundary
    creating build\lib.win-amd64-3.8\commonroad_dc\collision
    copying commonroad_dc\collision\__init__.py -> build\lib.win-amd64-3.8\commonroad_dc\collision
    creating build\lib.win-amd64-3.8\commonroad_dc\collision\collision_detection
    copying commonroad_dc\collision\collision_detection\__init__.py -> build\lib.win-amd64-3.8\commonroad_dc\collision\collision_detection
    copying commonroad_dc\collision\collision_detection\minkowski_sum.py -> build\lib.win-amd64-3.8\commonroad_dc\collision\collision_detection
    copying commonroad_dc\collision\collision_detection\pycrcc_collision_dispatch.py -> build\lib.win-amd64-3.8\commonroad_dc\collision\collision_detection
    copying commonroad_dc\collision\collision_detection\scenario.py -> build\lib.win-amd64-3.8\commonroad_dc\collision\collision_detection
    creating build\lib.win-amd64-3.8\commonroad_dc\collision\trajectory_queries
    copying commonroad_dc\collision\trajectory_queries\trajectory_queries.py -> build\lib.win-amd64-3.8\commonroad_dc\collision\trajectory_queries
    copying commonroad_dc\collision\trajectory_queries\trajectory_queries_specialized.py -> build\lib.win-amd64-3.8\commonroad_dc\collision\trajectory_queries
    creating build\lib.win-amd64-3.8\commonroad_dc\collision\visualization
    copying commonroad_dc\collision\visualization\__init__.py -> build\lib.win-amd64-3.8\commonroad_dc\collision\visualization
    copying commonroad_dc\collision\visualization\drawing.py -> build\lib.win-amd64-3.8\commonroad_dc\collision\visualization
    creating build\lib.win-amd64-3.8\commonroad_dc\costs
    copying commonroad_dc\costs\__init__.py -> build\lib.win-amd64-3.8\commonroad_dc\costs
    copying commonroad_dc\costs\evaluation.py -> build\lib.win-amd64-3.8\commonroad_dc\costs
    copying commonroad_dc\costs\partial_cost_functions.py -> build\lib.win-amd64-3.8\commonroad_dc\costs
    copying commonroad_dc\costs\route_matcher.py -> build\lib.win-amd64-3.8\commonroad_dc\costs
    creating build\lib.win-amd64-3.8\commonroad_dc\feasibility
    copying commonroad_dc\feasibility\__init__.py -> build\lib.win-amd64-3.8\commonroad_dc\feasibility
    copying commonroad_dc\feasibility\feasibility_checker.py -> build\lib.win-amd64-3.8\commonroad_dc\feasibility
    copying commonroad_dc\feasibility\solution_checker.py -> build\lib.win-amd64-3.8\commonroad_dc\feasibility
    copying commonroad_dc\feasibility\vehicle_dynamics.py -> build\lib.win-amd64-3.8\commonroad_dc\feasibility
    creating build\lib.win-amd64-3.8\commonroad_dc\geometry
    copying commonroad_dc\geometry\__init__.py -> build\lib.win-amd64-3.8\commonroad_dc\geometry
    copying commonroad_dc\geometry\geometry.py -> build\lib.win-amd64-3.8\commonroad_dc\geometry
    copying commonroad_dc\geometry\lanelet_ccosy.py -> build\lib.win-amd64-3.8\commonroad_dc\geometry
    copying commonroad_dc\geometry\util.py -> build\lib.win-amd64-3.8\commonroad_dc\geometry
    running build_ext
    -- Building for: Visual Studio 16 2019
    -- Selecting Windows SDK version 10.0.19041.0 to target Windows 10.0.19043.
    -- The C compiler identification is MSVC 19.29.30037.0
    -- The CXX compiler identification is MSVC 19.29.30037.0
    -- Detecting C compiler ABI info
    -- Detecting C compiler ABI info - done
    -- Check for working C compiler: C:/Program Files (x86)/Microsoft Visual Studio/2019/Community/VC/Tools/MSVC/14.29.30037/bin/Hostx64/x64/cl.exe - skipped
    -- Detecting C compile features
    -- Detecting C compile features - done
    -- Detecting CXX compiler ABI info
    -- Detecting CXX compiler ABI info - done
    -- Check for working CXX compiler: C:/Program Files (x86)/Microsoft Visual Studio/2019/Community/VC/Tools/MSVC/14.29.30037/bin/Hostx64/x64/cl.exe - skipped
    -- Detecting CXX compile features
    -- Detecting CXX compile features - done
    -- Configuring done
    -- Generating done
    -- Build files have been written to: C:/Users/Tong/AppData/Local/Temp/pip-install-jdzwspsk/commonroad-drivability-checker_1f5efd72f4dd4e98b5d7dd24fdbc71f8/build/temp.win-amd64-3.8/Release/build
    Microsoft (R) Build Engine version 16.10.1+2fd48ab73 for .NET Framework
    Copyright (C) Microsoft Corporation. All rights reserved.

    MSBUILD : error MSB1004: Specify the name of the target.
    Switch: --target

    For switch syntax, type "MSBuild -help"
    Traceback (most recent call last):
      File "<string>", line 1, in <module>
      File "C:\Users\Tong\AppData\Local\Temp\pip-install-jdzwspsk\commonroad-drivability-checker_1f5efd72f4dd4e98b5d7dd24fdbc71f8\setup.py", line 139, in <module>
        setup(
      File "C:\ProgramData\Anaconda3\envs\cmRd\lib\site-packages\setuptools\__init__.py", line 153, in setup
        return distutils.core.setup(**attrs)
      File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\core.py", line 148, in setup
        dist.run_commands()
      File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\dist.py", line 966, in run_commands
        self.run_command(cmd)
      File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\dist.py", line 985, in run_command
        cmd_obj.run()
      File "C:\ProgramData\Anaconda3\envs\cmRd\lib\site-packages\setuptools\command\install.py", line 61, in run
        return orig.install.run(self)
      File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\command\install.py", line 545, in run
        self.run_command('build')
      File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\cmd.py", line 313, in run_command
        self.distribution.run_command(command)
      File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\dist.py", line 985, in run_command
        cmd_obj.run()
      File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\command\build.py", line 135, in run
        self.run_command(cmd_name)
      File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\cmd.py", line 313, in run_command
        self.distribution.run_command(command)
      File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\dist.py", line 985, in run_command
        cmd_obj.run()
      File "C:\Users\Tong\AppData\Local\Temp\pip-install-jdzwspsk\commonroad-drivability-checker_1f5efd72f4dd4e98b5d7dd24fdbc71f8\setup.py", line 42, in run
        self.build_extension(ext)
      File "C:\Users\Tong\AppData\Local\Temp\pip-install-jdzwspsk\commonroad-drivability-checker_1f5efd72f4dd4e98b5d7dd24fdbc71f8\setup.py", line 118, in build_extension
        subprocess.check_call(['cmake', '--build', '.'] + build_args, cwd=build_dir)
      File "C:\ProgramData\Anaconda3\envs\cmRd\lib\subprocess.py", line 364, in check_call
        raise CalledProcessError(retcode, cmd)
    subprocess.CalledProcessError: Command '['cmake', '--build', '.', '--config', 'Release', '--', '/m', '--target', 'install']' returned non-zero exit status 1.
    ['-DADD_PYTHON_BINDINGS=TRUE', '-DADD_TESTS=OFF', '-DBUILD_DOC=OFF', '-DPYTHON_INCLUDE_DIR=C:\\ProgramData\\Anaconda3\\envs\\cmRd\\Include', '-DPYTHON_LIBRARY=', '-DPYTHON_EXECUTABLE=C:\\ProgramData\\Anaconda3\\envs\\cmRd\\python.exe']
    ----------------------------------------
ERROR: Command errored out with exit status 1: 'C:\ProgramData\Anaconda3\envs\cmRd\python.exe' -u -c 'import io, os, sys, setuptools, tokenize; sys.argv[0] = '"'"'C:\\Users\\Tong\\AppData\\Local\\Temp\\pip-install-jdzwspsk\\commonroad-drivability-checker_1f5efd72f4dd4e98b5d7dd24fdbc71f8\\setup.py'"'"'; __file__='"'"'C:\\Users\\Tong\\AppData\\Local\\Temp\\pip-install-jdzwspsk\\commonroad-drivability-checker_1f5efd72f4dd4e98b5d7dd24fdbc71f8\\setup.py'"'"';f = getattr(tokenize, '"'"'open'"'"', open)(__file__) if os.path.exists(__file__) else io.StringIO('"'"'from setuptools import setup; setup()'"'"');code = f.read().replace('"'"'\r\n'"'"', '"'"'\n'"'"');f.close();exec(compile(code, __file__, '"'"'exec'"'"'))' install --record 'C:\Users\Tong\AppData\Local\Temp\pip-record-levpxnqh\install-record.txt' --single-version-externally-managed --compile --install-headers 'C:\ProgramData\Anaconda3\envs\cmRd\Include\commonroad-drivability-checker' Check the logs for full command output.

(cmRd) C:\Users\Tong>
```
