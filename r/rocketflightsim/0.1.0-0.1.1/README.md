# Comparing `tmp/rocketflightsim-0.1.0.tar.gz` & `tmp/rocketflightsim-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rocketflightsim-0.1.0.tar", last modified: Wed May 22 17:42:50 2024, max compression
+gzip compressed data, was "rocketflightsim-0.1.1.tar", last modified: Mon May 27 00:47:28 2024, max compression
```

## Comparing `rocketflightsim-0.1.0.tar` & `rocketflightsim-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 17:42:50.069535 rocketflightsim-0.1.0/
--rw-rw-rw-   0        0        0     1095 2024-05-22 17:42:28.000000 rocketflightsim-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      784 2024-05-22 17:42:50.068538 rocketflightsim-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      262 2024-05-22 17:42:28.000000 rocketflightsim-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 17:42:50.031111 rocketflightsim-0.1.0/examples/
--rw-rw-rw-   0        0        0        0 2024-05-22 17:42:28.000000 rocketflightsim-0.1.0/examples/__init__.py
--rw-rw-rw-   0        0        0    32789 2024-05-22 17:42:28.000000 rocketflightsim-0.1.0/examples/test_configs.py
-drwxrwxrwx   0        0        0        0 2024-05-22 17:42:50.047075 rocketflightsim-0.1.0/rocketflightsim/
--rw-rw-rw-   0        0        0      353 2024-05-22 17:42:28.000000 rocketflightsim-0.1.0/rocketflightsim/__init__.py
--rw-rw-rw-   0        0        0     1710 2024-05-22 17:42:28.000000 rocketflightsim-0.1.0/rocketflightsim/constants.py
--rw-rw-rw-   0        0        0    15752 2024-05-22 17:42:28.000000 rocketflightsim-0.1.0/rocketflightsim/flight_simulation.py
--rw-rw-rw-   0        0        0     7900 2024-05-22 17:42:28.000000 rocketflightsim-0.1.0/rocketflightsim/helper_functions.py
--rw-rw-rw-   0        0        0    14888 2024-05-22 17:42:28.000000 rocketflightsim-0.1.0/rocketflightsim/plotting_functions.py
--rw-rw-rw-   0        0        0     5377 2024-05-22 17:42:28.000000 rocketflightsim-0.1.0/rocketflightsim/rocket_classes.py
-drwxrwxrwx   0        0        0        0 2024-05-22 17:42:50.063552 rocketflightsim-0.1.0/rocketflightsim.egg-info/
--rw-rw-rw-   0        0        0      784 2024-05-22 17:42:49.000000 rocketflightsim-0.1.0/rocketflightsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2024-05-22 17:42:50.000000 rocketflightsim-0.1.0/rocketflightsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 17:42:49.000000 rocketflightsim-0.1.0/rocketflightsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-22 17:42:49.000000 rocketflightsim-0.1.0/rocketflightsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2024-05-22 17:42:49.000000 rocketflightsim-0.1.0/rocketflightsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 17:42:50.069535 rocketflightsim-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      778 2024-05-22 17:42:28.000000 rocketflightsim-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 17:42:50.067566 rocketflightsim-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2024-05-22 17:42:28.000000 rocketflightsim-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     1342 2024-05-22 17:42:28.000000 rocketflightsim-0.1.0/tests/test_flight_simulation.py
+drwxrwxrwx   0        0        0        0 2024-05-27 00:47:28.322411 rocketflightsim-0.1.1/
+-rw-rw-rw-   0        0        0     1095 2024-05-25 02:16:59.000000 rocketflightsim-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      784 2024-05-27 00:47:28.322411 rocketflightsim-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2024-05-25 02:16:59.000000 rocketflightsim-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 00:47:28.262432 rocketflightsim-0.1.1/examples/
+-rw-rw-rw-   0        0        0        0 2024-05-25 02:16:59.000000 rocketflightsim-0.1.1/examples/__init__.py
+-rw-rw-rw-   0        0        0     7943 2024-05-27 00:45:43.000000 rocketflightsim-0.1.1/examples/example_configurations.py
+drwxrwxrwx   0        0        0        0 2024-05-27 00:47:28.278516 rocketflightsim-0.1.1/rocketflightsim/
+-rw-rw-rw-   0        0        0      353 2024-05-27 00:14:19.000000 rocketflightsim-0.1.1/rocketflightsim/__init__.py
+-rw-rw-rw-   0        0        0     1350 2024-05-25 04:59:23.000000 rocketflightsim-0.1.1/rocketflightsim/constants.py
+-rw-rw-rw-   0        0        0    16006 2024-05-26 22:52:51.000000 rocketflightsim-0.1.1/rocketflightsim/flight_simulation.py
+-rw-rw-rw-   0        0        0     8603 2024-05-26 22:52:51.000000 rocketflightsim-0.1.1/rocketflightsim/helper_functions.py
+-rw-rw-rw-   0        0        0    14888 2024-05-25 02:16:59.000000 rocketflightsim-0.1.1/rocketflightsim/plotting_functions.py
+-rw-rw-rw-   0        0        0     9342 2024-05-26 22:52:51.000000 rocketflightsim-0.1.1/rocketflightsim/rocket_classes.py
+drwxrwxrwx   0        0        0        0 2024-05-27 00:47:28.315425 rocketflightsim-0.1.1/rocketflightsim.egg-info/
+-rw-rw-rw-   0        0        0      784 2024-05-27 00:47:28.000000 rocketflightsim-0.1.1/rocketflightsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2024-05-27 00:47:28.000000 rocketflightsim-0.1.1/rocketflightsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 00:47:28.000000 rocketflightsim-0.1.1/rocketflightsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-27 00:47:28.000000 rocketflightsim-0.1.1/rocketflightsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2024-05-27 00:47:28.000000 rocketflightsim-0.1.1/rocketflightsim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 00:47:28.323406 rocketflightsim-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      778 2024-05-27 00:11:50.000000 rocketflightsim-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 00:47:28.320457 rocketflightsim-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-25 02:16:59.000000 rocketflightsim-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0    30829 2024-05-27 00:25:53.000000 rocketflightsim-0.1.1/tests/test_configs.py
+-rw-rw-rw-   0        0        0     3194 2024-05-27 00:25:33.000000 rocketflightsim-0.1.1/tests/test_flight_simulation.py
```

### Comparing `rocketflightsim-0.1.0/LICENSE` & `rocketflightsim-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rocketflightsim-0.1.0/PKG-INFO` & `rocketflightsim-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocketflightsim
-Version: 0.1.0
+Version: 0.1.1
 Summary: A lightweight rocket flight simulator.
 Home-page: https://github.com/werocketry/RocketFlightSim
 Author: Giorgio Chassikos, Western Engineering Rocketry Team
 Author-email: werocketry@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rocketflightsim-0.1.0/examples/test_configs.py` & `rocketflightsim-0.1.1/tests/test_configs.py`

 * *Files 10% similar despite different names*

```diff
@@ -320,21 +320,22 @@
     # fuel mass curve couldn't be found, so will make one
     # initial mass is 1.409 kg (from GitHub), final mass is 0 kg
     # total impulse is 1415.154 Ns (from GitHub)
         # verified to be the same value as taking the integral of the thrust curve
     # make the fuel burn speed proportional to the thrust
 )
 total_impulse = 1415.154
+times = list(keron.thrust_curve.keys())
 for i in range(1, len(keron.thrust_curve)):
-    keron.fuel_mass_curve[list(keron.thrust_curve.keys())[i]] = keron.fuel_mass_curve[list(keron.thrust_curve.keys())[i-1]] - (keron.thrust_curve[list(keron.thrust_curve.keys())[i]] + keron.thrust_curve[list(keron.thrust_curve.keys())[i-1]])/2 * (list(keron.thrust_curve.keys())[i] - list(keron.thrust_curve.keys())[i-1]) / total_impulse * 1.409
+    keron.fuel_mass_curve[times[i]] = keron.fuel_mass_curve[times[i-1]] - (keron.thrust_curve[times[i]] + keron.thrust_curve[times[i-1]])/2 * (times[i] - times[i-1]) / total_impulse * 1.409
 """ # Visualization of the fuel mass curve compared to the thrust curve
 # plot the fuel burn speed and the thrust on the same graph (different scales)
 import matplotlib.pyplot as plt
 fig, ax1 = plt.subplots()
-ax1.plot(list(keron.thrust_curve.keys()), [keron.thrust_curve[i] for i in keron.thrust_curve], 'b-')
+ax1.plot(times, [keron.thrust_curve[i] for i in keron.thrust_curve], 'b-')
 ax1.set_xlabel('time (s)')
 ax1.set_ylabel('Thrust (N)', color='b')
 ax1.tick_params('y', colors='b')
 ax2 = ax1.twinx()
 ax2.plot(list(keron.fuel_mass_curve.keys()), [keron.fuel_mass_curve[i] for i in keron.fuel_mass_curve], 'r-')
 ax2.set_ylabel('Fuel mass (kg)', color='r')
 ax2.tick_params('y', colors='r')
@@ -911,76 +912,27 @@
 )
 Bella_Lui_flight = PastFlight(
     rocket=Bella_Lui_rocket,
     launch_conditions=Bella_Lui_launch_conditions,
     apogee=458.97,
     name="Bella Lui 2020"
 )
-"""
+""" TODO: investigate why the sim performs so poorly on this flight compared to the others
 This is the flight that the sim is furthest off from predicting well. Possible reasons:
 - weak motor, short and quick flight leads to:
     - various small effects not accounted for in the sim made more significant
     - can't put the energy into wording it right now, but intuition
+    - try simulating from burnout to apogee to see if the sim is more accurate there
+    - would wind have a larger effect?
 - not confident in the values the notebook provides for the motor:
     - adding on the motor mass from thrustcurve.org, the sim gives an error of -14.76, instead of +24.63
         - also lended some credence due to the sim also underestimating the other 3 flights
     - was it even the K828FJ that was used?
         - the RocketPy paper says that total impulse of the "class K solid motor" used for the flight was 2120 Ns, but the notebook says 2070.99 Ns
             - https://www.researchgate.net/publication/354034513_RocketPy_Six_Degree-of-Freedom_Rocket_Trajectory_Simulator
 - using a constant Cd may not be a great approximation for a rocket hitting about Mach 0.25 
     - also, no mention of where the Cd value comes from. If it's ork or RasAero, it's likely not accurate. If it was CFD, they likely would have given a curve
-
+- no local variation in lapse rate from the standard lapse rate accounted for. Based on how it affects a 10k launch, it can improve the accuracy by about 0.3%, which might be another small factor
 Could diagnose more by comparing plots of data from the flight computer to plots from the sim, but a bit busy atm
 """
-# Lapse rate gives a 10k launch about a 30ft difference, and g gives it about a 10ft difference, so it could account for a decent amount of the error. Though I suspect it may be overoptimistic to assume that the sim is that accurate. Still need to do a proper error analysis
-
-past_flights = [NDRT_2020_flight, Valetudo_flight, Juno3_flight, Bella_Lui_flight]
-
-default_airbrakes_model = Airbrakes(
-    num_flaps = 3,
-    A_flap = 0.00395,  # m^2  flap area
-    Cd_brakes = 1,
-    max_deployment_speed = 5.5,  # deg/s
-    max_deployment_angle = 45  # deg
-)
-""" Currently taken from airbrakes_model_2024_03_20 in team's airbrakes repo
-TODO: eventually replace with something that feels like a good default
-"""
-
-if __name__ == "__main__":
-    from rocketflightsim.flight_simulation import FlightSimulation as fsim
-
-    for past_flight in past_flights:
-        print(f"Rocket: {past_flight.name}")
-        apogee = fsim.simulate_flight(past_flight.rocket, past_flight.launch_conditions, timestep = 0.001)[0]['height'].iloc[-1]
-        print(f"\tApogee prediction: {apogee:.2f} m")
-        print(f"\tActual apogee: {past_flight.apogee:.2f} m")
-        print(f"\tError: {apogee - past_flight.apogee:.2f} m")
-        print(f"\tPercent error: {(apogee - past_flight.apogee)/past_flight.apogee*100:.2f} %")
-        # note that the sim doesn't account for wind yet, will bring predicted apogee down
-
-    # past_flight = Juno3_flight
-    # # plot the flight
-    # import plotting_functions as pf
-    # (
-    #         dataset,
-    #         liftoff_index,
-    #         launch_rail_cleared_index,
-    #         burnout_index,
-    #         apogee_index,
-    # ) = fsim.simulate_flight(past_flight.rocket, past_flight.launch_conditions, timestep = 0.001)
-
-    # time = dataset["time"][:apogee_index]
-    # height = dataset["height"][:apogee_index].copy()
-    # speed = dataset["speed"][:apogee_index].copy()
-    # v_y = dataset["v_y"][:apogee_index].copy()
-    # a_y = dataset["a_y"][:apogee_index].copy()
-    # a_x = dataset["a_x"][:apogee_index].copy()
 
-    # pf.plot_aerodynamics(
-    #         time,
-    #         height,
-    #         speed,
-    #         dataset["q"],
-    #         dataset["angle_to_vertical"],
-    #         dataset["air_density"],
-    #         )
+past_flights = [NDRT_2020_flight, Valetudo_flight, Juno3_flight, Bella_Lui_flight]
```

### Comparing `rocketflightsim-0.1.0/rocketflightsim/flight_simulation.py` & `rocketflightsim-0.1.1/rocketflightsim/flight_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,26 +35,28 @@
     fuel_mass_lookup = rocket.motor.fuel_mass_curve
     engine_thrust_lookup = rocket.motor.thrust_curve
     Cd_A_rocket_fn = rocket.Cd_A_rocket
     burnout_time = rocket.motor.burn_time
 
     # Extract launch condition parameters
     launchpad_pressure = launch_conditions.launchpad_pressure
-    launchpad_temp = launch_conditions.launchpad_temp + 273.15
+    launchpad_temp = launch_conditions.launchpad_temp
     L_launch_rail = launch_conditions.L_launch_rail
     launch_angle = launch_conditions.launch_angle
+    
     T_lapse_rate = launch_conditions.local_T_lapse_rate
+    F_gravity = launch_conditions.local_gravity
 
     # Initialize simulation variables
     time, height, speed, a_y, a_x, v_y, v_x, Cd_A_rocket, Ma, q = 0, 0, 0, 0, 0, 0, 0, 0, 0, 0
     angle_to_vertical = np.deg2rad(90 - launch_angle)
-
     # Calculate constants to be used in air density function, set initial air density
-    multiplier = launchpad_pressure / (con.R_specific_air * pow(launchpad_temp, con.F_g_over_R_spec_air_T_lapse_rate))
-    air_density = hfunc.air_density_optimized(launchpad_temp, multiplier)
+    multiplier = launchpad_pressure / (con.R_specific_air * pow(launchpad_temp, - F_gravity / (con.R_specific_air * T_lapse_rate)))
+    exponent = - F_gravity / (con.R_specific_air * T_lapse_rate) - 1
+    air_density = hfunc.air_density_optimized(launchpad_temp, multiplier, exponent)
 
     # Store the initial state of the rocket
     simulated_values = [
         [
             time,
             height,
             speed,
@@ -71,15 +73,15 @@
         ]
     ]
 
     # Simulate motor burn until liftoff
     while (
         hfunc.thrust_at_time(time, engine_thrust_lookup)
         / hfunc.mass_at_time(time, dry_mass, fuel_mass_lookup)
-        <= con.F_gravity
+        <= F_gravity
     ):
         time += timestep
         # Append simulation values for each timestep
         simulated_values.append(
             [
                 time,
                 height, # 0
@@ -104,26 +106,26 @@
     effective_L_launch_rail = L_launch_rail - rocket.h_second_rail_button
     effective_h_launch_rail = effective_L_launch_rail * np.cos(angle_to_vertical)
 
     # Simulate flight from liftoff until the launch rail is cleared
     while height < effective_h_launch_rail:
         # Update environmental conditions based on height
         temperature = hfunc.temp_at_height(height, launchpad_temp, lapse_rate = T_lapse_rate)
-        air_density = hfunc.air_density_optimized(temperature, multiplier)
+        air_density = hfunc.air_density_optimized(temperature, multiplier,exponent)
 
         # Calculate Mach number, drag coefficient, and forces
         Ma = hfunc.mach_number_fn(speed, temperature)
         Cd_A_rocket = Cd_A_rocket_fn(Ma)
         q = hfunc.calculate_dynamic_pressure(air_density, speed)
         F_drag = q * Cd_A_rocket
 
         # Update rocket's motion parameters
         mass = hfunc.mass_at_time(time, dry_mass, fuel_mass_lookup)
         thrust = hfunc.thrust_at_time(time, engine_thrust_lookup)
-        a_y = (thrust - F_drag) * np.cos(angle_to_vertical) / mass - con.F_gravity
+        a_y = (thrust - F_drag) * np.cos(angle_to_vertical) / mass - F_gravity
         a_x = (thrust - F_drag) * np.sin(angle_to_vertical) / mass
         v_y += a_y * timestep
         v_x += a_x * timestep
         speed = np.sqrt(v_y**2 + v_x**2)
         height += v_y * timestep
 
         # Append updated simulation values
@@ -148,26 +150,26 @@
 
     launch_rail_cleared_index = len(simulated_values)
 
     # Flight from launch rail cleared until burnout
     while time < burnout_time:
         # Update environmental conditions based on height
         temperature = hfunc.temp_at_height(height, launchpad_temp, lapse_rate = T_lapse_rate)
-        air_density = hfunc.air_density_optimized(temperature, multiplier)
+        air_density = hfunc.air_density_optimized(temperature, multiplier,exponent)
 
         # Calculate Mach number, Drag coefficient, and Forces
         Ma = hfunc.mach_number_fn(speed, temperature)
         Cd_A_rocket = Cd_A_rocket_fn(Ma)
         q = hfunc.calculate_dynamic_pressure(air_density, speed)
         F_drag = q * Cd_A_rocket
 
         # Update rocket's motion parameters
         mass = hfunc.mass_at_time(time, dry_mass, fuel_mass_lookup)
         thrust = hfunc.thrust_at_time(time, engine_thrust_lookup)
-        a_y = (thrust - F_drag) * np.cos(angle_to_vertical) / mass - con.F_gravity
+        a_y = (thrust - F_drag) * np.cos(angle_to_vertical) / mass - F_gravity
         a_x = (thrust - F_drag) * np.sin(angle_to_vertical) / mass
         v_y += a_y * timestep
         v_x += a_x * timestep
         speed = np.sqrt(v_y**2 + v_x**2)
         height += v_y * timestep
 
         # Recalculate the angle to the veritcal
@@ -197,24 +199,24 @@
     burnout_index = len(simulated_values)
 
     # Flight from burnout to apogee
     mass = dry_mass
 
     while v_y > 0:
         temperature = hfunc.temp_at_height(height, launchpad_temp, lapse_rate = T_lapse_rate)
-        air_density = hfunc.air_density_optimized(temperature, multiplier)
+        air_density = hfunc.air_density_optimized(temperature, multiplier,exponent)
 
         # Calculate Mach number, Drag coefficient, and Forces
         Ma = hfunc.mach_number_fn(speed, temperature)
         Cd_A_rocket = Cd_A_rocket_fn(Ma)
         q = hfunc.calculate_dynamic_pressure(air_density, speed)
         F_drag = q * Cd_A_rocket
 
         # Update rocket's motion parameters
-        a_y = -F_drag * np.cos(angle_to_vertical) / mass - con.F_gravity
+        a_y = -F_drag * np.cos(angle_to_vertical) / mass - F_gravity
         a_x = -F_drag * np.sin(angle_to_vertical) / mass
         v_y += a_y * timestep
         v_x += a_x * timestep
         speed = np.sqrt(v_y**2 + v_x**2)
         height += v_y * timestep
 
         # Recalculate the angle to the veritcal
@@ -291,18 +293,21 @@
     # Extract rocket parameters
     mass = rocket.dry_mass
     Cd_A_rocket_fn = rocket.Cd_A_rocket
 
     # Extract launch condition parameters
     launchpad_temp = pre_brake_flight.temperature.iloc[0]
     launchpad_pressure = pre_brake_flight.air_density.iloc[0] * con.R_specific_air * launchpad_temp
-    T_lapse_rate = launch_conditions.local_T_lapse_rate
+    
+    T_lapse_rate = launch_conditions.local_T_lapse_rate    
+    F_gravity = launch_conditions.local_gravity
 
     # Calculate constants to be used in air density function
-    multiplier = launchpad_pressure / (con.R_specific_air * pow(launchpad_temp, con.F_g_over_R_spec_air_T_lapse_rate))
+    multiplier = launchpad_pressure / (con.R_specific_air * pow(launchpad_temp, - F_gravity / (con.R_specific_air * T_lapse_rate)))
+    exponent = - F_gravity / (con.R_specific_air * T_lapse_rate) - 1
 
     # Extract airbrakes parameters
     Cd_brakes = airbrakes.Cd_brakes
     max_deployment_speed = np.deg2rad(airbrakes.max_deployment_speed)
     max_deployment_angle = np.deg2rad(airbrakes.max_deployment_angle)
     A_brakes = airbrakes.num_flaps * airbrakes.A_flap
 
@@ -323,28 +328,28 @@
     A_Cd_brakes = A_brakes * Cd_brakes
 
     simulated_values = []
     while v_y > 0:
         time += timestep
 
         temperature = hfunc.temp_at_height(height, launchpad_temp, lapse_rate = T_lapse_rate)
-        air_density = hfunc.air_density_optimized(temperature, multiplier)
+        air_density = hfunc.air_density_optimized(temperature, multiplier,exponent)
         Ma = hfunc.mach_number_fn(speed, temperature)
         Cd_A_rocket = Cd_A_rocket_fn(Ma)
         q = hfunc.calculate_dynamic_pressure(air_density, speed)
 
         deployment_angle = min(max_deployment_angle, deployment_angle + max_deployment_speed * timestep)
 
         if deployment_angle >= max_deployment_angle and not time_recorded:
             time_of_max_deployment = time
             time_recorded = True
 
 
         F_drag = q * (np.sin(deployment_angle) * A_Cd_brakes + Cd_A_rocket)
-        a_y = -F_drag * np.cos(angle_to_vertical) / mass - con.F_gravity
+        a_y = -F_drag * np.cos(angle_to_vertical) / mass - F_gravity
         a_x = -F_drag * np.sin(angle_to_vertical) / mass
         v_y += a_y * timestep
         v_x += a_x * timestep
         speed = np.sqrt(v_y**2 + v_x**2)
         height += v_y * timestep
 
         angle_to_vertical = np.arctan(v_x / v_y)
@@ -391,17 +396,14 @@
 
     if not time_recorded:
         time_of_max_deployment = time
 
     return ascent, time_of_max_deployment
 
 
-if __name__ == "__main__":
-    pass 
-
 # TODO: move this to a test file
     # run a couple hundred different timesteps in logspace between 0.001 and 0.1 to see how it changes to help pick a good timestep
     
 """    apogees = []
     for timestep in np.logspace(-3, -1, 200):
         dataset, liftoff_index, launch_rail_cleared_index, burnout_index, apogee_index = simulate_flight(rocket=Juno3_rocket, timestep=timestep)
         ascent, time_of_max_deployment = simulate_airbrakes_flight(dataset.iloc[:burnout_index].copy(), rocket=Juno3_rocket, launch_conditions=Juno3_launch_conditions, timestep=0.001)
```

### Comparing `rocketflightsim-0.1.0/rocketflightsim/helper_functions.py` & `rocketflightsim-0.1.1/rocketflightsim/helper_functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,38 @@
 import numpy as np
 from . import constants as con
 
 # aerodynamics
 def temp_at_height(h, launchpad_temp, lapse_rate = con.T_lapse_rate):
     """
-    Calculate the temperature at a given height above the launchpad.
+    Calculate the temperature at a given height above the launchpad. Within the troposphere, the temperature decreases linearly with height at a rate known as the lapse rate. The lapse rate is typically around 6.5 degrees Celsius per kilometer. 
 
     Args:
     - h (float): Height above the launchpad in meters.
     - launchpad_temp (float): Temperature at the launchpad in Celsius or Kelvin.
+    - lapse_rate (float, optional): Rate at which temperature decreases with height in degrees Celsius or Kelvin per meter. Defaults to the standard lapse rate of 0.0065.
 
     Returns:
     - float: Temperature at the given height in Celsius or Kelvin (same as input).
     """
     return launchpad_temp + (h * lapse_rate)
-def pressure_at_height(h, launchpad_temp, launchpad_pressure):
-    """
-    Calculate the air pressure at a given height above the launchpad.
-
-    Args:
-    - h (float): Height above the launchpad in meters.
-    - launchpad_temp (float): Temperature at the launchpad in Kelvin.
-    - launchpad_pressure (float): Air pressure at the launchpad in Pascals.
-
-    Returns:
-    - float: Air pressure at the given height in Pascals.
-    """
-    return launchpad_pressure * pow(
-        (1 - (h * con.T_lapse_rate / launchpad_temp)),
-        (con.F_g_over_R_spec_air_T_lapse_rate)
-    )
-def air_density_fn(pressure, temp):
-    """
-    Calculate the density of air at a given pressure and temperature.
-
-    Args:
-    - pressure (float): Pressure in Pascals.
-    - temp (float): Temperature in Kelvin.
 
-    Returns:
-    - float: Air density in kilograms per cubic meter.
-    """
-    return pressure / (con.R_specific_air * temp)
-def air_density_optimized(temp, multiplier):
+def air_density_optimized(temp, multiplier, exponent):
     """
     Calculate the density of air at a given height above the launchpad.
 
     Args:
     - temp (float): Temperature at the given height in Kelvin.
-    - multiplier (float): A constant derived from the temperature and pressure at the launchpad, the lapse rate, the specific gas constant for air, and the value for gravity near the Earth's surface. Calculated at the start of the simulation script outside of the main loops. Equal to P_launchpad / (R_air * pow(T_launchpad, Fg_over_R_spec_air_T_lapse_rate)).
+    - multiplier (float): A constant derived from the temperature and pressure at the launchpad, the lapse rate, the specific gas constant for air, and the magnitude of the force of gravity. Calculated at the start of the simulation script outside of the main loops. Equal to P_launchpad / (R_air * pow(T_launchpad, - F_gravity / (R_air * T_lapse_rate))).
+    - exponent (float): A constant derived from the lapse rate, the specific gas constant for air, and the magnitude of the force of gravity. Calculated at the start of the simulation script outside of the main loops. Equal to - F_gravity / (R_air * T_lapse_rate) - 1.
 
     Returns:
     - float: Air density at the given height in kilograms per cubic meter.
     """
-    return multiplier * pow(temp, con.F_g_over_R_spec_air_T_lapse_rate_minus_one)
+    return multiplier * pow(temp, exponent)
 
 def calculate_dynamic_pressure(air_density, speed):
     """
     Calculate the dynamic pressure imparted on a solid moving through a fluid.
 
     Args:
     - air_density (float): The density of the fluid.
@@ -116,15 +91,45 @@
 
     if h_expected:
         g_apogee = gamma_0 * (1 - (k1 - k2 * np.sin(phi)**2) * h_expected + k3 * h_expected**2)
         return (g_launchpad + g_apogee) / 2
     else:
         return g_launchpad
 
-# not used anymore
+# not used in simulator
+def pressure_at_height(h, launchpad_temp, launchpad_pressure):
+    """
+    Calculate the air pressure at a given height above the launchpad.
+
+    Args:
+    - h (float): Height above the launchpad in meters.
+    - launchpad_temp (float): Temperature at the launchpad in Kelvin.
+    - launchpad_pressure (float): Air pressure at the launchpad in Pascals.
+
+    Returns:
+    - float: Air pressure at the given height in Pascals.
+    """ # note, could use a specific sim's local gravity and lapse rate to be more accurate
+    return launchpad_pressure * pow(
+        (1 - (h * con.T_lapse_rate / launchpad_temp)),
+        (con.F_gravity / (con.R_specific_air * con.T_lapse_rate))
+    )
+
+def air_density_fn(pressure, temp):
+    """
+    Calculate the density of air at a given pressure and temperature.
+
+    Args:
+    - pressure (float): Pressure in Pascals.
+    - temp (float): Temperature in Kelvin.
+
+    Returns:
+    - float: Air density in kilograms per cubic meter.
+    """
+    return pressure / (con.R_specific_air * temp)
+
 def lookup_dynamic_viscosity(temp):
     """
     Look up the dynamic viscosity of air at a given temperature.
 
     Args:
     - temp (float): Temperature in Kelvin.
 
@@ -137,14 +142,15 @@
     # Lookup table for dynamic viscosity
     temps = np.array([173.15, 223.15, 233.15, 243.15, 253.15, 263.15, 273.15, 278.15, 283.15, 288.15, 293.15, 298.15, 303.15, 308.15, 313.15, 318.15, 323.15, 333.15, 343.15])
     viscosities = np.array([1.189e-6, 1.474e-5, 1.527e-5, 1.579e-5, 1.630e-5, 1.680e-5, 1.729e-5, 1.754e-5, 1.778e-5, 1.802e-5, 1.825e-5, 1.849e-5, 1.872e-5, 1.895e-5, 1.918e-5, 1.941e-5, 1.963e-5, 2.008e-5, 2.052e-5])
     
     # Interpolate
     viscosity = np.interp(temp, temps, viscosities)
     return viscosity
+
 def calculate_reynolds_number(air_density, speed, len_characteristic, dynamic_viscosity):
     """
     Calculate the Reynolds number of a solid moving through air.
 
     Args:
     - air_density (float): The density of the air.
     - speed (float): The relative speed of the solid and the air.
```

### Comparing `rocketflightsim-0.1.0/rocketflightsim/plotting_functions.py` & `rocketflightsim-0.1.1/rocketflightsim/plotting_functions.py`

 * *Files identical despite different names*

### Comparing `rocketflightsim-0.1.0/rocketflightsim.egg-info/PKG-INFO` & `rocketflightsim-0.1.1/rocketflightsim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rocketflightsim
-Version: 0.1.0
+Version: 0.1.1
 Summary: A lightweight rocket flight simulator.
 Home-page: https://github.com/werocketry/RocketFlightSim
 Author: Giorgio Chassikos, Western Engineering Rocketry Team
 Author-email: werocketry@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rocketflightsim-0.1.0/rocketflightsim.egg-info/SOURCES.txt` & `rocketflightsim-0.1.1/rocketflightsim.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 LICENSE
 README.md
 setup.py
 examples/__init__.py
-examples/test_configs.py
+examples/example_configurations.py
 rocketflightsim/__init__.py
 rocketflightsim/constants.py
 rocketflightsim/flight_simulation.py
 rocketflightsim/helper_functions.py
 rocketflightsim/plotting_functions.py
 rocketflightsim/rocket_classes.py
 rocketflightsim.egg-info/PKG-INFO
 rocketflightsim.egg-info/SOURCES.txt
 rocketflightsim.egg-info/dependency_links.txt
 rocketflightsim.egg-info/requires.txt
 rocketflightsim.egg-info/top_level.txt
 tests/__init__.py
+tests/test_configs.py
 tests/test_flight_simulation.py
```

### Comparing `rocketflightsim-0.1.0/setup.py` & `rocketflightsim-0.1.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rocketflightsim',
-    version='0.1.0',
+    version='0.1.1',
     description='A lightweight rocket flight simulator.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Giorgio Chassikos, Western Engineering Rocketry Team',
     author_email='werocketry@gmail.com',
     url='https://github.com/werocketry/RocketFlightSim',
     packages=find_packages(),
```

