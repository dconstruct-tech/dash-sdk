# SCRIPT API REFERENCE
d.ASH Nav supports custom scripting by the user, allowing the user to edit what functions are called at certain waypoints. The way d.ASH Nav allows for this is through it's own scripting API.

---

#### Missions

<details>
 <summary><code>clearMission()</code> <code>Clears all current missions</code></summary>

<b>Parameters</b>

<table>
<tr>
<th>Name</th>
<th>description</th>
</tr>
<tr>
<td>N/A</td>
<td>N/A</td>
</tr>
</table>

</details>

<details>
 <summary><code>setMissionName(string missionName, bool upload)</code> <code>Creates new mission, call before any mission is run</code></summary>

<b>Parameters</b>

<table>
<tr>
<th>Name</th>
<th>description</th>
</tr>
<tr>
<td>missionName</td>
<td>Name of mission</td>
</tr>
<tr>
<td>upload</td>
<td>Upload status to cloud (Default: False)</td>
</tr>
</table>

</details>

---

#### Waypoints

<details>
 <summary><code>endWaypoint()</code> <code>Command issued to end autonomous movement. Must be the last action called if <i>waypoint3D</i> is used</code></summary>

<b>Parameters</b>

<table>
<tr>
<th>Name</th>
<th>description</th>
</tr>
<tr>
<td>N/A</td>
<td>N/A</td>
</tr>
</table>

</details>

<details>
 <summary><code>waypoint3D(int seg, float x, float y, float z)</code> <code>Makes robot move to a specific coordinate on a map</code></summary>

<b>Parameters</b>

<table>
<tr>
<th>Name</th>
<th>description</th>
</tr>
<tr>
<td>seg</td>
<td>Segment of path. Set as zero</td>
</tr>
<tr>
<td>x</td>
<td>X coordinate on the map</td>
</tr>
<tr>
<td>y</td>
<td>Y coordinate on the map</td>
</tr>
<tr>
<td>z</td>
<td>Z coordinate on the map (Height)</td>
</tr>
</table>

</details>

<details>
 <summary><code>capture(int camID)</code> <code>Takes an image for camera specified in <i>camID</i></code></summary>

<b>Parameters</b>

<table>
<tr>
<th>Name</th>
<th>description</th>
</tr>
<tr>
<td>camID</td>
<td>ID of camera used</td>
</tr>
</table>

</details>

<details>
 <summary><code>capturePano(string fileName)</code> <code>Takes a panoramic image and saves it as <i>fileName</i>.jpg</code></summary>

<b>Parameters</b>

<table>
<tr>
<th>Name</th>
<th>description</th>
</tr>
<tr>
<td>fileName</td>
<td>Name of file</td>
</tr>
</table>

</details>

<details>
 <summary><code>DockingAction(bool isDockOn)</code> <code><b>EXPERIMENTAL | BOSDYN SPOT ONLY | </b>Pauses robot movement and docks robot</code></summary>

<b>Parameters</b>

<table>
<tr>
<th>Name</th>
<th>description</th>
</tr>
<tr>
<td>isDockOn</td>
<td>If docking is supported on the robot</td>
</tr>
</table>

</details>

<details>
 <summary><code>AutoDocking(bool isDockOn)</code> <code>Pauses robot movement and docks robot</code></summary>

<b>Parameters</b>

<table>
<tr>
<th>Name</th>
<th>description</th>
</tr>
<tr>
<td>isDockOn</td>
<td>If docking is supported on the robot</td>
</tr>
</table>

</details>

<details>
 <summary><code>pause(int dur)</code> <code>Pauses robot movement for <i>dur</i> seconds</code></summary>

<b>Parameters</b>

<table>
<tr>
<th>Name</th>
<th>description</th>
</tr>
<tr>
<td>dur</td>
<td>Time in seconds to pause the robot for</td>
</tr>
</table>

</details>

<details>
 <summary><code>scanRTC(string jobName, int res, bool enableImaging, bool enableDoubleScan, bool enableVis)</code> <code>Sets robot to scan using Leica™ RTC360 at a selected waypoint</code></summary>

<b>Parameters</b>

<table>
<tr>
<th>Name</th>
<th>description</th>
</tr>
<tr>
<td>jobName</td>
<td>Name of scan job</td>
</tr>
<tr>
<td>res</td>
<td>Resolution of scan</td>
</tr>
<tr>
<td>enableImaging</td>
<td>Whether to scan with colour (imaging)</td>
</tr>
<tr>
<td>enableDoubleScan</td>
<td>Enable Leica™ Double scan</td>
</tr>
<tr>
<td>enableVis</td>
<td>Enable Leica™ Visual Inertial System</td>
</tr>
</table>

</details>

<details>
 <summary><code>scanBLK(string jobName, int res, int imgQly, bool stream)</code> <code>Sets robot to scan using Leica™ BLK360 at a selected waypoint</code></summary>

<b>Parameters</b>

<table>
<tr>
<th>Name</th>
<th>description</th>
</tr>
<tr>
<td>jobName</td>
<td>Name of scan job</td>
</tr>
<tr>
<td>res</td>
<td>Resolution of scan</td>
</tr>
<tr>
<td>imgQly</td>
<td>Image quality to scan at</td>
</tr>
<tr>
<td>stream</td>
<td>Enable streaming of files to d.ASH Xplorer</td>
</tr>
</table>

</details>

<details>
 <summary><code>scanARC(bool isStart)</code> <code>Sets robot to scan using Leica™ BLK ARC at a selected waypoint</code></summary>

<b>Parameters</b>

<table>
<tr>
<th>Name</th>
<th>description</th>
</tr>
<tr>
<td>isStart</td>
<td>Start or stop scanning</td>
</tr>
</table>

</details>
