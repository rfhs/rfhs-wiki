## Virtual Foxhunt
### Quick Start:
To access the virtual foxhunt, please go here: [http://dfsim.net/index.php](http://dfsim.net/index.php)

### Direction of Arrival (DOA)/Angle of Arrival (AOA):
The DOA portion of the Virtual Foxhunt uses simulated transmitters and receivers. You are provided with receiver location and signal angle of arrival data. Your task is to collect and process that data to determine the location of the transmitter.

The easy version of this challenge will require some basic math and will allow you simply draw lines on a map to locate the target. The intermediate and hard versions of this challenge deal with moving receivers and transmitters, therefore you'll be required to aggregate and analyze the data.

Researching the following topics can help push you in the right direction:
- Great Circle Intersections
- Vincenty and Haversine Equations

### Time Difference of Arrival (TDOA):
The TDOA portion of the Virtual Foxhunt provides a sample of IQ data and an information file for each receiver. You task is to find the time delay between each receiver and use that information to determine the location of the transmitter. Don't worry about decoding the signal, it's randomly generated.

The "easy" version of the challenge will provide you with both the IQ data and pre-computed time differences. The intermediate version of the challenge will only provide the IQ data, leaving you to find the time difference yourself.