# SCRIPT API REFERENCE
d.ASH Nav supports custom scripting by the user, allowing the user to edit what functions are called at certain waypoints. The way d.ASH Nav allows for this is through it's own scripting API.

---

#### Missions

<details>
 <summary><code>clearMission()</code> <code>Clears all current missions</code></summary>

##### Parameters

> | name | description |
> |----|----|
> | N/A | N/A |

</details>

<details>
 <summary><code>setMissionName(string missionName, bool upload)</code> <code>Creates new mission, call before any mission is run</code></summary>

##### Parameters

> | name | description |
> |----|----|
> | missionName | Name of mission |
> | upload | Upload status to cloud (Default: False) |

</details>

---

#### Waypoints

<details>
 <summary><code>endWaypoint()</code> <code>Command issued to end autonomous movement. Must be the last action called if <i>waypoint3D</i> is used</code></summary>

##### Parameters

> | name | description |
> |----|----|
> | N/A | N/A |

</details>

<details>
 <summary><code>waypoint3D(int seg, float x, float y, float z)</code> <code>Makes robot move to a specific coordinate on a map</code></summary>

##### Parameters

> | name | description |
> |----|----|
> | seg | Segment of path. Set as zero |
> | x | X coordinate on the map |
> | y | Y coordinate on the map |
> | z | Z coordinate on the map (Height) |

</details>

<details>
 <summary><code>capture(int camID)</code> <code>Takes an image for camera specified in <i>camID</i></code></summary>

##### Parameters

> | name | description |
> |----|----|
> | camID | ID of camera used |

</details>

<details>
 <summary><code>capturePano(string fileName)</code> <code>Takes a panoramic image and saves it as <i>fileName</i>.jpg</code></summary>

##### Parameters

> | name | description |
> |----|----|
> | fileName | Name of file |

</details>

<details>
 <summary><code>DockingAction(bool isDockOn)</code> <code><b>EXPERIMENTAL | BOSDYN SPOT ONLY | </b>Pauses robot movement and docks robot</code></summary>

##### Parameters

> | name | description |
> |----|----|
> | isDockOn | If docking is supported on the robot |

</details>

<details>
 <summary><code>AutoDocking(bool isDockOn)</code> <code>Pauses robot movement and docks robot</code></summary>

##### Parameters

> | name | description |
> |----|----|
> | isDockOn | If docking is supported on the robot |

</details>

<details>
 <summary><code>pause(int dur)</code> <code>Pauses robot movement for <i>dur</i> seconds</code></summary>

##### Parameters

> | name | description |
> |----|----|
> | dur | Time in seconds to pause the robot for |

</details>

<details>
 <summary><code>scanRTC(string jobName, int res, bool enableImaging, bool enableDoubleScan, bool enableVis)</code> <code>Sets robot to scan using Leica™ RTC360 at a selected waypoint</code></summary>

##### Parameters

> | name | description |
> |----|----|
> | jobName | Name of scan job |
> | res | Resolution of scan |
> | enableImaging | Whether to scan with colour (imaging) |
> | enableDoubleScan | Enable Leica™ Double scan |
> | enableVis | Enable Leica™ Visual Inertial System |

</details>

<details>
 <summary><code>scanBLK(string jobName, int res, int imgQly)</code> <code>Sets robot to scan using Leica™ BLK360 at a selected waypoint</code></summary>

##### Parameters

> | name | description |
> |----|----|
> | jobName | Name of scan job |
> | res | Resolution of scan |
> | imgQly | Image quality to scan at |

</details>

<details>
 <summary><code>scanARC(bool isStart)</code> <code>Sets robot to scan using Leica™ BLK ARC at a selected waypoint</code></summary>

##### Parameters

> | name | description |
> |----|----|
> | isStart | Start or stop scanning |

</details>
