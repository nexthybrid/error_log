# Error log of driveability-checker build in Windows 10

The following is an error log when I was trying to follow the guide at the [doc](https://commonroad.in.tum.de/docs/commonroad-drivability-checker/sphinx/installation.html#method-2-manual-installation) to manually build driveability-checker on Windows 10.

```
(cmRd) C:\github\commonroad-drivability-checker>BUILD_JOBS=8 python setup.py build
'BUILD_JOBS' is not recognized as an internal or external command,
operable program or batch file.

(cmRd) C:\github\commonroad-drivability-checker>python setup.py build
C:\ProgramData\Anaconda3\envs\cmRd\lib\site-packages\setuptools\dist.py:717: UserWarning: Usage of dash-separated 'description-file' will not be supported in future versions. Please use the underscore name 'description_file' instead
  warnings.warn(
running build
running build_py
creating build
creating build\lib.win-amd64-3.8
creating build\lib.win-amd64-3.8\commonroad_dc
copying commonroad_dc\__init__.py -> build\lib.win-amd64-3.8\commonroad_dc
running egg_info
creating commonroad_drivability_checker.egg-info
writing commonroad_drivability_checker.egg-info\PKG-INFO
writing dependency_links to commonroad_drivability_checker.egg-info\dependency_links.txt
writing requirements to commonroad_drivability_checker.egg-info\requires.txt
writing top-level names to commonroad_drivability_checker.egg-info\top_level.txt
writing manifest file 'commonroad_drivability_checker.egg-info\SOURCES.txt'
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
['-DADD_PYTHON_BINDINGS=TRUE', '-DADD_TESTS=OFF', '-DBUILD_DOC=OFF', '-DPYTHON_INCLUDE_DIR=C:\\ProgramData\\Anaconda3\\envs\\cmRd\\Include', '-DPYTHON_LIBRARY=', '-DPYTHON_EXECUTABLE=C:\\ProgramData\\Anaconda3\\envs\\cmRd\\python.exe']
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
-- Build files have been written to: C:/github/commonroad-drivability-checker/build/temp.win-amd64-3.8/Release/build
Microsoft (R) Build Engine version 16.10.1+2fd48ab73 for .NET Framework
Copyright (C) Microsoft Corporation. All rights reserved.

MSBUILD : error MSB1004: Specify the name of the target.
Switch: --target

For switch syntax, type "MSBuild -help"
Traceback (most recent call last):
  File "setup.py", line 139, in <module>
    setup(
  File "C:\ProgramData\Anaconda3\envs\cmRd\lib\site-packages\setuptools\__init__.py", line 153, in setup
    return distutils.core.setup(**attrs)
  File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\core.py", line 148, in setup
    dist.run_commands()
  File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\dist.py", line 966, in run_commands
    self.run_command(cmd)
  File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\dist.py", line 985, in run_command
    cmd_obj.run()
  File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\command\build.py", line 135, in run
    self.run_command(cmd_name)
  File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\cmd.py", line 313, in run_command
    self.distribution.run_command(command)
  File "C:\ProgramData\Anaconda3\envs\cmRd\lib\distutils\dist.py", line 985, in run_command
    cmd_obj.run()
  File "setup.py", line 42, in run
    self.build_extension(ext)
  File "setup.py", line 118, in build_extension
    subprocess.check_call(['cmake', '--build', '.'] + build_args, cwd=build_dir)
  File "C:\ProgramData\Anaconda3\envs\cmRd\lib\subprocess.py", line 364, in check_call
    raise CalledProcessError(retcode, cmd)
subprocess.CalledProcessError: Command '['cmake', '--build', '.', '--config', 'Release', '--', '/m', '--target', 'install']' returned non-zero exit status 1.

(cmRd) C:\github\commonroad-drivability-checker>
```