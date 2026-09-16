Interactive Edge AI poster source

1. Keep index.html, system-architecture.jpg and confusion_matrix.png in the same folder.
2. Open index.html in a modern browser to preview it.
3. Select "Run inspection" to follow the normal route: Camera -> Raspberry Pi -> Image Processing -> Offload Decision -> Local YOLO11n -> Flask Dashboard -> Results Log.
4. After the local route completes, select "Simulate high CPU load". A new frame starts at Camera -> Raspberry Pi -> Image Processing -> Decision. After CPU reaches >=90% for 60 seconds, the JPEG frame changes to Base64/JSON and follows MQTT Broker -> Cloud YOLO -> MQTT Broker -> Flask Dashboard -> Results Log.
5. Use "Pause animation" at any point during an inspection and "Resume animation" to continue from the same point.
6. Keyboard controls: Tab moves through controls; Enter/Space opens accordions and flips result cards; Left/Right/Home/End changes tabs.
7. Replace the footer's demo URL placeholder and QR placeholder with the final public demonstration URL and matching QR code.
8. Upload all three files together when replacing the current GitHub Pages source.

The 60-second sustained CPU threshold is visually accelerated in the demonstration. The displayed implementation rule remains CPU >=90% for 60 seconds.
The page respects the system's reduced-motion preference and removes non-essential movement when it is enabled.
