**OBD Simulator**
Command line utility to simulate and send data on 127.0.0.1:11333 in format required for obdlogger "/src/sbc-car/src/logger".

**OBD Logger database structure**
Tables: **ecu**, **gps**, **obd**, **trip**.

1. Table **ecu**:
	* **ecuid** (INTEGER);
	* **vin** (TEXT);
	* **ecu** (INTEGER);
	* **ecudesc** (TEXT);
2. Table **gps**:
	* **lat** (REAL);
	* **lon** (REAL);
	* **alt** (REAL);
	* **speed** (REAL);
	* **course** (REAL);
	* **gpstime** (REAL);
	* **time** (REAL);
	* **trip** (INTEGER);
3. Table **obd**:
	* **time** (REAL);
	* **trip** (INTEGER);
	* **ecu** (INTEGER);
4. Table **trip**:
	* **tripid** (INTEGER);
	* **start** (REAL);
	* **end** (REAL);
