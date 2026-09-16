Interactive Edge AI poster source

1. Keep index.html, system-architecture.jpg and confusion_matrix.png in the same folder.
2. Open index.html in a modern browser to preview it.
3. Select "Run inspection" to follow the normal route: Camera -> Raspberry Pi -> Image Processing -> Offload Decision -> Local YOLO11n -> Flask Dashboard -> Results Log.
4. After the local route completes, select "Simulate high CPU load" to follow the offload route: Decision -> MQTT Broker -> Cloud YOLO -> MQTT Broker -> Flask Dashboard -> Results Log.
5. Upload all three files together when replacing the current GitHub Pages source.

The 60-second sustained CPU threshold is visually accelerated in the demonstration. The displayed implementation rule remains CPU >=90% for 60 seconds.
