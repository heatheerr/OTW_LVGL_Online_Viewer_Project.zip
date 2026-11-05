# OTW LVGL Online Viewer — matched to your uploaded driver HTML

I used the uploaded `index_driver_updated_fixed(2).html` as the visual source.

## What is matched
- Original dark maroon/red background and left navigation sidebar
- OTW brand area and Dashboard / Navigation / Request / Passengers sections
- Dashboard structure: L300 vehicle card, Shuttle 01, Standby, ABC 1234
- Passenger Status card, 0/8 count, remaining seats and seat icons
- Start Trip / End Trip controls
- Current Route with Lessandra Heights, En Route, Vista Mall Daang Hari
- Request tabs and passenger request card layout
- Passenger occupancy list
- Navigation banner and bottom Remaining / ETA / Current Speed metrics
- Trip Completed summary page
- 1024 x 600 target for Waveshare ESP32-S3-Touch-LCD-7B

## Important difference
The `reference/original_driver.html` and `reference/exact_browser_preview.html` are your original HTML copied unchanged. Open `exact_browser_preview.html` in Edge/Chrome to see the exact original interface.

The XML screens are a **native LVGL visual recreation**, not a pixel-perfect or behavior-complete conversion. LVGL does not render HTML/CSS directly. The XML pages use matching layout and text but need validation in LVGL Online Viewer; the map is a placeholder, and live backend actions are not connected in the XML preview. The original HTML still contains your live web-app code and Cloudflare API integration.

## Online Viewer
The LVGL Online Viewer does not directly open a local ZIP. Upload the project folder contents to a public GitHub repository (keep `project.xml`, `globals.xml`, and `screens/` at repository root), then open https://viewer.lvgl.io/ and load the repository URL.

Reference: https://lvgl.io/docs/open/9.4/details/xml/tools/online_share.html
