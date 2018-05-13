# TestBenchmarks
Comparing NUnit &amp; xunit. Each run is 10 000 tests with a trivial assert.

[![xunit](https://ci.appveyor.com/api/projects/status/2xikxwbm422fxys9/branch/XUnit?svg=true)](https://ci.appveyor.com/project/JohanLarsson/testbenchmarks/branch/XUnit)
[![NUnit](https://ci.appveyor.com/api/projects/status/2xikxwbm422fxys9/branch/NUnit?svg=true)](https://ci.appveyor.com/project/JohanLarsson/testbenchmarks/branch/NUnit)

<table>
  <tr>
    <td>Total time</td>
    <td><a href="https://www.nuget.org/packages/NUnit/3.10.1">NUnit</a></td>
    <td><a href="https://www.nuget.org/packages/xunit/2.3.1">xunit</a></td>
  </tr>
  <tr>
    <td>Visual studio runner</td>
    <td><a href="https://user-images.githubusercontent.com/1640096/39966263-1b430cb0-56a9-11e8-9917-c9aa8b5ed1b8.gif">18.4 s</a></td>
    <td><a href="https://user-images.githubusercontent.com/1640096/39966274-57c66984-56a9-11e8-8818-0515e68f2d42.gif">42.0 s</a></td>
  </tr>
  <tr>
    <td>Resharper runner</td>
    <td><a href="https://user-images.githubusercontent.com/1640096/39966289-8ab128c0-56a9-11e8-9718-828d5f557223.gif">53.6 s</a></td>
    <td><a href="https://user-images.githubusercontent.com/1640096/39966295-b5fb89d0-56a9-11e8-85bc-a24b4bfc31ad.gif">61.6 s</a></td>
  </tr>
  <tr>
    <td>Rider</td>
    <td><a href="https://user-images.githubusercontent.com/1640096/39966305-ee1cb2a8-56a9-11e8-9e9e-06927cf505ac.gif">48.6 s</a></td>
    <td><a href="https://user-images.githubusercontent.com/1640096/39966313-0c775064-56aa-11e8-88d3-d3cec499c431.gif">64 s</a></td>
  </tr>
  <tr>
    <td>AppVeyor</td>
    <td><a href="https://ci.appveyor.com/project/JohanLarsson/testbenchmarks/build/1.0.7">6 min 13 s</a></td>
    <td><a href="https://ci.appveyor.com/project/JohanLarsson/testbenchmarks/build/1.0.6">4 min 22 s</a></td>
  </tr>    
<table>

The times in the table link to a screen recording of the run.

## How the benchmarks were run
1. Git clean
2. Open the editor and let it resolve references.
3. Set Release|AnyCPU
4. Start recording using [ScreenToGif](http://www.screentogif.com/) and start test run.

### Environment
Visual Studio Enterprise 15.7.1
JetBrains Resharper Ultimate 2018.1
NUnit 3.10.1
NUnit 3 Test Adapter 3.10.0.0
xunit 2.3.1
Rider 2018.1
Intel Xeon CPU E5-2637 v4 3.50GHz, 2 CPU, 16 logical and 8 physical cores

