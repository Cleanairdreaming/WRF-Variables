.. WRF-variables documentation master file, created by
   sphinx-quickstart on Fri Dec  6 14:53:02 2019.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to WRF-variables's documentation!
=========================================

.. toctree::
   :maxdepth: 2
   :caption: Contents:



Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

WRF-variables
==============

Times
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
str Times(Time, DateStrLen)
  | unlimited dimensions: Time
  | current shape = (1, 19)
  | filling on, default _FillValue of   used

时间。

XLAT
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>

float32 XLAT(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: LATITUDE, SOUTH IS NEGATIVE
  | units: degree_north
  | stagger: 
  | coordinates: XLONG XLAT
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

纬度。单位°，南纬是负值。

XLONG
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 XLONG(Time, south_north, west_east)::
  | FieldType: 104
  | MemoryOrder: XY 
  | description: LONGITUDE, WEST IS NEGATIVE
  | units: degree_east
  | stagger: 
  | coordinates: XLONG XLAT
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

经度。单位°，西经是负值。

LU_INDEX
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 LU_INDEX(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: LAND USE CATEGORY
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

地面使用类型。无单位。

ZNU
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 ZNU(Time, bottom_top)
  | FieldType: 104
  | MemoryOrder: Z  
  | description: eta values on half (mass) levels
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1, 29)
  | filling on, default _FillValue of 9.969209968386869e+36 used

半层的eta值（质量层）。

ZNW
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 ZNW(Time, bottom_top_stag)
  | FieldType: 104
  | MemoryOrder: Z  
  | description: eta values on full (w) levels
  | units: 
  | stagger: Z
  | unlimited dimensions: Time
  | current shape = (1, 30)
  | filling on, default _FillValue of 9.969209968386869e+36 used

全层的eta值（w层）。

ZS
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 ZS(Time, soil_layers_stag)
  | FieldType: 104
  | MemoryOrder: Z  
  | description: DEPTHS OF CENTERS OF SOIL LAYERS
  | units: m
  | stagger: Z
  | unlimited dimensions: Time
  | current shape = (1, 4)
  | filling on, default _FillValue of 9.969209968386869e+36 used

土壤层中心深度，m。

DZS
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 DZS(Time, soil_layers_stag)
  | FieldType: 104
  | MemoryOrder: Z  
  | description: THICKNESSES OF SOIL LAYERS
  | units: m
  | stagger: Z
  | unlimited dimensions: Time
  | current shape = (1, 4)
  | filling on, default _FillValue of 9.969209968386869e+36 used

土壤层厚度，m。

VAR_SSO
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 VAR_SSO(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: variance of subgrid-scale orography
  | units: m2
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

亚网格尺度的地形变化，m。

LAP_HGT
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 LAP_HGT(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: Laplacian of orography
  | units: m
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

拉普拉斯地形，m。

U
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 U(Time, bottom_top, south_north, west_east_stag)
  | FieldType: 104
  | MemoryOrder: XYZ
  | description: x-wind component
  | units: m s-1
  | stagger: X
  | coordinates: XLONG_U XLAT_U XTIME
  | unlimited dimensions: Time
  | current shape = (1, 29, 21, 22)
  | filling on, default _FillValue of 9.969209968386869e+36 used

x-方向风分量，m/s。

V
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 V(Time, bottom_top, south_north_stag, west_east)
  | FieldType: 104
  | MemoryOrder: XYZ
  | description: y-wind component
  | units: m s-1
  | stagger: Y
  | coordinates: XLONG_V XLAT_V XTIME
  | unlimited dimensions: Time
  | current shape = (1, 29, 22, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

y方向风分量，m/s。

W
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 W(Time, bottom_top_stag, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XYZ
  | description: z-wind component
  | units: m s-1
  | stagger: Z
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 30, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

z方向风分量，m/s。

PH
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 PH(Time, bottom_top_stag, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XYZ
  | description: perturbation geopotential
  | units: m2 s-2
  | stagger: Z
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 30, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

位势扰动，m2/s-2。

PHB
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 PHB(Time, bottom_top_stag, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XYZ
  | description: base-state geopotential
  | units: m2 s-2
  | stagger: Z
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 30, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

基态位势，m2/s-2。

T
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 T(Time, bottom_top, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XYZ
  | description: perturbation potential temperature (theta-t0)
  | units: K
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 29, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

HFX_FORCE
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 HFX_FORCE(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: SCM ideal surface sensible heat flux
  | units: W m-2
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

LH_FORCE
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 LH_FORCE(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: SCM ideal surface latent heat flux
  | units: W m-2
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

TSK_FORCE
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 TSK_FORCE(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: SCM ideal surface skin temperature
  | units: W m-2
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

HFX_FORCE_TEND
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 HFX_FORCE_TEND(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: SCM ideal surface sensible heat flux tendency
  | units: W m-2 s-1
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

LH_FORCE_TEND
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 LH_FORCE_TEND(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: SCM ideal surface latent heat flux tendency
  | units: W m-2 s-1
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

TSK_FORCE_TEND
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 TSK_FORCE_TEND(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: SCM ideal surface skin temperature tendency
  | units: W m-2 s-1
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

MU
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 MU(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: perturbation dry air mass in column
  | units: Pa
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

MUB
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 MUB(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: base state dry air mass in column
  | units: Pa
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

NEST_POS
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 NEST_POS(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: -
  | units: -
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

P
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 P(Time, bottom_top, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XYZ
  | description: perturbation pressure
  | units: Pa
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 29, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

PB
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 PB(Time, bottom_top, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XYZ
  | description: BASE STATE PRESSURE
  | units: Pa
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 29, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

FNM
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 FNM(Time, bottom_top)
  | FieldType: 104
  | MemoryOrder: Z  
  | description: upper weight for vertical stretching
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1, 29)
  | filling on, default _FillValue of 9.969209968386869e+36 used

FNP
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 FNP(Time, bottom_top)
  | FieldType: 104
  | MemoryOrder: Z  
  | description: lower weight for vertical stretching
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1, 29)
  | filling on, default _FillValue of 9.969209968386869e+36 used

RDNW
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 RDNW(Time, bottom_top)
  | FieldType: 104
  | MemoryOrder: Z  
  | description: inverse d(eta) values between full (w) levels
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1, 29)
  | filling on, default _FillValue of 9.969209968386869e+36 used

RDN
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 RDN(Time, bottom_top)
  | FieldType: 104
  | MemoryOrder: Z  
  | description: inverse d(eta) values between half (mass) levels
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1, 29)
  | filling on, default _FillValue of 9.969209968386869e+36 used

DNW
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 DNW(Time, bottom_top)
  | FieldType: 104
  | MemoryOrder: Z  
  | description: d(eta) values between full (w) levels
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1, 29)
  | filling on, default _FillValue of 9.969209968386869e+36 used

DN
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 DN(Time, bottom_top)
  | FieldType: 104
  | MemoryOrder: Z  
  | description: d(eta) values between half (mass) levels
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1, 29)
  | filling on, default _FillValue of 9.969209968386869e+36 used

CFN
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 CFN(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: extrapolation constant
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

CFN1
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 CFN1(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: extrapolation constant
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

THIS_IS_AN_IDEAL_RUN
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
int32 THIS_IS_AN_IDEAL_RUN(Time)
  | FieldType: 106
  | MemoryOrder: 0  
  | description: T/F flag: this is an ARW ideal simulation
  | units: -
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of -2147483647 used

P_HYD
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 P_HYD(Time, bottom_top, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XYZ
  | description: hydrostatic pressure
  | units: Pa
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 29, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

Q2
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 Q2(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: QV at 2 M
  | units: kg kg-1
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

T2
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 T2(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: TEMP at 2 M
  | units: K
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

TH2
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 TH2(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: POT TEMP at 2 M
  | units: K
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

PSFC
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 PSFC(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: SFC PRESSURE
  | units: Pa
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

U10
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 U10(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: U at 10 M
  | units: m s-1
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

V10
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 V10(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: V at 10 M
  | units: m s-1
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

RDX
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 RDX(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: INVERSE X GRID LENGTH
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

RDY
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 RDY(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: INVERSE Y GRID LENGTH
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

RESM
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 RESM(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: TIME WEIGHT CONSTANT FOR SMALL STEPS
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

ZETATOP
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 ZETATOP(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: ZETA AT MODEL TOP
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

CF1
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 CF1(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: 2nd order extrapolation constant
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

CF2
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 CF2(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: 2nd order extrapolation constant
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

CF3
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 CF3(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: 2nd order extrapolation constant
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

ITIMESTEP
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
int32 ITIMESTEP(Time)
  | FieldType: 106
  | MemoryOrder: 0  
  | description: 
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of -2147483647 used

XTIME
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 XTIME(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: minutes since 2019-08-14 00:00:00
  | units: minutes since 2019-08-14 00:00:00
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

QVAPOR
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 QVAPOR(Time, bottom_top, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XYZ
  | description: Water vapor mixing ratio
  | units: kg kg-1
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 29, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

QCLOUD
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 QCLOUD(Time, bottom_top, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XYZ
  | description: Cloud water mixing ratio
  | units: kg kg-1
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 29, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

QRAIN
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 QRAIN(Time, bottom_top, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XYZ
  | description: Rain water mixing ratio
  | units: kg kg-1
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 29, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

SHDMAX
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 SHDMAX(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: ANNUAL MAX VEG FRACTION
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

SHDMIN
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 SHDMIN(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: ANNUAL MIN VEG FRACTION
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

SNOALB
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 SNOALB(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: ANNUAL MAX SNOW ALBEDO IN FRACTION
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

TSLB
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 TSLB(Time, soil_layers_stag, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XYZ
  | description: SOIL TEMPERATURE
  | units: K
  | stagger: Z
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 4, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

SMOIS
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 SMOIS(Time, soil_layers_stag, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XYZ
  | description: SOIL MOISTURE
  | units: m3 m-3
  | stagger: Z
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 4, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

SH2O
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 SH2O(Time, soil_layers_stag, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XYZ
  | description: SOIL LIQUID WATER
  | units: m3 m-3
  | stagger: Z
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 4, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

SMCREL
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 SMCREL(Time, soil_layers_stag, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XYZ
  | description: RELATIVE SOIL MOISTURE
  | units: 
  | stagger: Z
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 4, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

SEAICE
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 SEAICE(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: SEA ICE FLAG
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

XICEM
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 XICEM(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: SEA ICE FLAG (PREVIOUS STEP)
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

SFROFF
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 SFROFF(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: SURFACE RUNOFF
  | units: mm
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

UDROFF
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 UDROFF(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: UNDERGROUND RUNOFF
  | units: mm
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

IVGTYP
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
int32 IVGTYP(Time, south_north, west_east)
  | FieldType: 106
  | MemoryOrder: XY 
  | description: DOMINANT VEGETATION CATEGORY
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of -2147483647 used

ISLTYP
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
int32 ISLTYP(Time, south_north, west_east)
  | FieldType: 106
  | MemoryOrder: XY 
  | description: DOMINANT SOIL CATEGORY
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of -2147483647 used

VEGFRA
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 VEGFRA(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: VEGETATION FRACTION
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

GRDFLX
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 GRDFLX(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: GROUND HEAT FLUX
  | units: W m-2
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

ACGRDFLX
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 ACGRDFLX(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: ACCUMULATED GROUND HEAT FLUX
  | units: J m-2
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

ACSNOM
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 ACSNOM(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: ACCUMULATED MELTED SNOW
  | units: kg m-2
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

SNOW
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 SNOW(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: SNOW WATER EQUIVALENT
  | units: kg m-2
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

SNOWH
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 SNOWH(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: PHYSICAL SNOW DEPTH
  | units: m
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

CANWAT
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 CANWAT(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: CANOPY WATER
  | units: kg m-2
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

SSTSK
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 SSTSK(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: SKIN SEA SURFACE TEMPERATURE
  | units: K
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

COSZEN
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 COSZEN(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: COS of SOLAR ZENITH ANGLE
  | units: dimensionless
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

LAI
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 LAI(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: LEAF AREA INDEX
  | units: m-2/m-2
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

VAR
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 VAR(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: OROGRAPHIC VARIANCE
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

MAPFAC_M
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 MAPFAC_M(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: Map scale factor on mass grid
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

MAPFAC_U
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 MAPFAC_U(Time, south_north, west_east_stag)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: Map scale factor on u-grid
  | units: 
  | stagger: X
  | coordinates: XLONG_U XLAT_U XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 22)
  | filling on, default _FillValue of 9.969209968386869e+36 used

MAPFAC_V
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 MAPFAC_V(Time, south_north_stag, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: Map scale factor on v-grid
  | units: 
  | stagger: Y
  | coordinates: XLONG_V XLAT_V XTIME
  | unlimited dimensions: Time
  | current shape = (1, 22, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

MAPFAC_MX
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 MAPFAC_MX(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: Map scale factor on mass grid, x direction
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

MAPFAC_MY
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 MAPFAC_MY(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: Map scale factor on mass grid, y direction
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

MAPFAC_UX
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 MAPFAC_UX(Time, south_north, west_east_stag)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: Map scale factor on u-grid, x direction
  | units: 
  | stagger: X
  | coordinates: XLONG_U XLAT_U XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 22)
  | filling on, default _FillValue of 9.969209968386869e+36 used

MAPFAC_UY
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 MAPFAC_UY(Time, south_north, west_east_stag)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: Map scale factor on u-grid, y direction
  | units: 
  | stagger: X
  | coordinates: XLONG_U XLAT_U XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 22)
  | filling on, default _FillValue of 9.969209968386869e+36 used

MAPFAC_VX
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 MAPFAC_VX(Time, south_north_stag, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: Map scale factor on v-grid, x direction
  | units: 
  | stagger: Y
  | coordinates: XLONG_V XLAT_V XTIME
  | unlimited dimensions: Time
  | current shape = (1, 22, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

MF_VX_INV
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 MF_VX_INV(Time, south_north_stag, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: Inverse map scale factor on v-grid, x direction
  | units: 
  | stagger: Y
  | coordinates: XLONG_V XLAT_V XTIME
  | unlimited dimensions: Time
  | current shape = (1, 22, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

MAPFAC_VY
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 MAPFAC_VY(Time, south_north_stag, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: Map scale factor on v-grid, y direction
  | units: 
  | stagger: Y
  | coordinates: XLONG_V XLAT_V XTIME
  | unlimited dimensions: Time
  | current shape = (1, 22, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

F
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 F(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: Coriolis sine latitude term
  | units: s-1
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

E
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 E(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: Coriolis cosine latitude term
  | units: s-1
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

SINALPHA
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 SINALPHA(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: Local sine of map rotation
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

COSALPHA
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 COSALPHA(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: Local cosine of map rotation
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

HGT
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 HGT(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: Terrain Height
  | units: m
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

TSK
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 TSK(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: SURFACE SKIN TEMPERATURE
  | units: K
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

P_TOP
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 P_TOP(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: PRESSURE TOP OF THE MODEL
  | units: Pa
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

T00
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 T00(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: BASE STATE TEMPERATURE
  | units: K
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

P00
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 P00(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: BASE STATE PRESURE
  | units: Pa
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

TLP
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 TLP(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: BASE STATE LAPSE RATE
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

TISO
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 TISO(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: TEMP AT WHICH THE BASE T TURNS CONST
  | units: K
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

TLP_STRAT
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 TLP_STRAT(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: BASE STATE LAPSE RATE (DT/D(LN(P)) IN STRATOSPHERE
  | units: K
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

P_STRAT
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 P_STRAT(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: BASE STATE PRESSURE AT BOTTOM OF STRATOSPHERE
  | units: Pa
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

MAX_MSTFX
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 MAX_MSTFX(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: Max map factor in domain
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

MAX_MSTFY
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 MAX_MSTFY(Time)
  | FieldType: 104
  | MemoryOrder: 0  
  | description: Max map factor in domain
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of 9.969209968386869e+36 used

RAINC
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 RAINC(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: ACCUMULATED TOTAL CUMULUS PRECIPITATION
  | units: mm
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

RAINSH
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 RAINSH(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: ACCUMULATED SHALLOW CUMULUS PRECIPITATION
  | units: mm
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

RAINNC
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 RAINNC(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: ACCUMULATED TOTAL GRID SCALE PRECIPITATION
  | units: mm
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

SNOWNC
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 SNOWNC(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: ACCUMULATED TOTAL GRID SCALE SNOW AND ICE
  | units: mm
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

GRAUPELNC
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 GRAUPELNC(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: ACCUMULATED TOTAL GRID SCALE GRAUPEL
  | units: mm
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

HAILNC
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 HAILNC(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: ACCUMULATED TOTAL GRID SCALE HAIL
  | units: mm
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

CLDFRA
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 CLDFRA(Time, bottom_top, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XYZ
  | description: CLOUD FRACTION
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 29, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

SWDOWN
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 SWDOWN(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: DOWNWARD SHORT WAVE FLUX AT GROUND SURFACE
  | units: W m-2
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

GLW
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 GLW(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: DOWNWARD LONG WAVE FLUX AT GROUND SURFACE
  | units: W m-2
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

SWNORM
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 SWNORM(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: NORMAL SHORT WAVE FLUX AT GROUND SURFACE (SLOPE-DEPENDENT)
  | units: W m-2
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

DIFFUSE_FRAC
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 DIFFUSE_FRAC(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: DIFFUSE FRACTION OF SURFACE SHORTWAVE IRRADIANCE
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

OLR
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 OLR(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: TOA OUTGOING LONG WAVE
  | units: W m-2
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

XLAT_U
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 XLAT_U(Time, south_north, west_east_stag)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: LATITUDE, SOUTH IS NEGATIVE
  | units: degree_north
  | stagger: X
  | coordinates: XLONG_U XLAT_U
  | unlimited dimensions: Time
  | current shape = (1, 21, 22)
  | filling on, default _FillValue of 9.969209968386869e+36 used

XLONG_U
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 XLONG_U(Time, south_north, west_east_stag)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: LONGITUDE, WEST IS NEGATIVE
  | units: degree_east
  | stagger: X
  | coordinates: XLONG_U XLAT_U
  | unlimited dimensions: Time
  | current shape = (1, 21, 22)
  | filling on, default _FillValue of 9.969209968386869e+36 used

XLAT_V
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 XLAT_V(Time, south_north_stag, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: LATITUDE, SOUTH IS NEGATIVE
  | units: degree_north
  | stagger: Y
  | coordinates: XLONG_V XLAT_V
  | unlimited dimensions: Time
  | current shape = (1, 22, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

XLONG_V
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 XLONG_V(Time, south_north_stag, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: LONGITUDE, WEST IS NEGATIVE
  | units: degree_east
  | stagger: Y
  | coordinates: XLONG_V XLAT_V
  | unlimited dimensions: Time
  | current shape = (1, 22, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

ALBEDO
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 ALBEDO(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: ALBEDO
  | units: -
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

CLAT
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 CLAT(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: COMPUTATIONAL GRID LATITUDE, SOUTH IS NEGATIVE
  | units: degree_north
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

ALBBCK
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 ALBBCK(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: BACKGROUND ALBEDO
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

EMISS
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 EMISS(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: SURFACE EMISSIVITY
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

NOAHRES
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 NOAHRES(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: RESIDUAL OF THE NOAH SURFACE ENERGY BUDGET
  | units: W m{-2}
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

TMN
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 TMN(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: SOIL TEMPERATURE AT LOWER BOUNDARY
  | units: K
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

XLAND
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 XLAND(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: LAND MASK (1 FOR LAND, 2 FOR WATER)
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

UST
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 UST(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: U* IN SIMILARITY THEORY
  | units: m s-1
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

PBLH
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 PBLH(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: PBL HEIGHT
  | units: m
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

HFX
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 HFX(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: UPWARD HEAT FLUX AT THE SURFACE
  | units: W m-2
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

QFX
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 QFX(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: UPWARD MOISTURE FLUX AT THE SURFACE
  | units: kg m-2 s-1
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

LH
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 LH(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: LATENT HEAT FLUX AT THE SURFACE
  | units: W m-2
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

ACHFX
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 ACHFX(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: ACCUMULATED UPWARD HEAT FLUX AT THE SURFACE
  | units: J m-2
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

ACLHF
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 ACLHF(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: ACCUMULATED UPWARD LATENT HEAT FLUX AT THE SURFACE
  | units: J m-2
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

SNOWC
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 SNOWC(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: FLAG INDICATING SNOW COVERAGE (1 FOR SNOW COVER)
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

SR
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 SR(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: fraction of frozen precipitation
  | units: -
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

SAVE_TOPO_FROM_REAL
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
int32 SAVE_TOPO_FROM_REAL(Time)
  | FieldType: 106
  | MemoryOrder: 0  
  | description: 1=original topo from real/0=topo modified by WRF
  | units: flag
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1,)
  | filling on, default _FillValue of -2147483647 used

ISEEDARR_RAND_PERTURB
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
int32 ISEEDARR_RAND_PERTURB(Time, bottom_top)
  | FieldType: 106
  | MemoryOrder: Z  
  | description: Array to hold seed for restart, RAND_PERT
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1, 29)
  | filling on, default _FillValue of -2147483647 used

ISEEDARR_SPPT
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
int32 ISEEDARR_SPPT(Time, bottom_top)
  | FieldType: 106
  | MemoryOrder: Z  
  | description: Array to hold seed for restart, SPPT
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1, 29)
  | filling on, default _FillValue of -2147483647 used

ISEEDARR_SKEBS
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
int32 ISEEDARR_SKEBS(Time, bottom_top)
  | FieldType: 106
  | MemoryOrder: Z  
  | description: Array to hold seed for restart, SKEBS
  | units: 
  | stagger: 
  | unlimited dimensions: Time
  | current shape = (1, 29)
  | filling on, default _FillValue of -2147483647 used

LANDMASK
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 LANDMASK(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: LAND MASK (1 FOR LAND, 0 FOR WATER)
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

LAKEMASK
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 LAKEMASK(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: LAKE MASK (1 FOR LAKE, 0 FOR NON-LAKE)
  | units: 
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

SST
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 SST(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: SEA SURFACE TEMPERATURE
  | units: K
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used

SST_INPUT
-----------------------------
::

<class 'netCDF4._netCDF4.Variable'>
float32 SST_INPUT(Time, south_north, west_east)
  | FieldType: 104
  | MemoryOrder: XY 
  | description: SEA SURFACE TEMPERATURE FROM WRFLOWINPUT FILE
  | units: K
  | stagger: 
  | coordinates: XLONG XLAT XTIME
  | unlimited dimensions: Time
  | current shape = (1, 21, 21)
  | filling on, default _FillValue of 9.969209968386869e+36 used


