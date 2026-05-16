# Telemetry Feature Documentation

This document explains telemetry feature extraction fields used by the ArduPilot AI Log Diagnosis pipeline.

## GPS Features

| Feature | Source | Meaning | Units / Notes |
|----------|---------|----------|----------------|
| gps_hdop_mean | GPS | Average GPS Horizontal Dilution of Precision | Lower values are better |
| gps_hdop_max | GPS | Maximum GPS precision deviation observed | HDOP |
| gps_nsats_mean | GPS | Average number of connected satellites | Count |
| gps_nsats_min | GPS | Minimum satellites available during flight | Count |
| gps_fix_pct | GPS | Percentage of flight with GPS fix available | Percentage |
| gps_hdop_tanomaly | GPS | Detects abnormal GPS precision spikes | Anomaly indicator |

## Vibration Features

| Feature | Source | Meaning | Units / Notes |
|----------|---------|----------|----------------|
| vibe_x_mean | VIBE | Average vibration on X-axis | Sensor value |
| vibe_y_mean | VIBE | Average vibration on Y-axis | Sensor value |
| vibe_z_mean | VIBE | Average vibration on Z-axis | Sensor value |
| vibe_x_max | VIBE | Maximum X-axis vibration | Sensor value |
| vibe_y_max | VIBE | Maximum Y-axis vibration | Sensor value |
| vibe_z_max | VIBE | Maximum Z-axis vibration | Sensor value |
| vibe_z_std | VIBE | Variation of Z-axis vibration | Standard deviation |
| vibe_clip_total | VIBE | Total vibration clipping events | Count |
| vibe_z_tanomaly | VIBE | Detects abnormal vibration spikes | Anomaly indicator |