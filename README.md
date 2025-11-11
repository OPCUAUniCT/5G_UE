# 5G_UE AAS — Asset Administration Shell for 5G User Equipment

This repository contains the **Asset Administration Shell (AAS)** model for a **5G User Equipment (UE)** device, packaged in the file `5G_UE.aasx`.  
The model has been developed as part of the *Water 4.0* project to integrate 5G mobile connectivity into the Digital Twin of an Integrated Water System (SII).

## Repository contents

- `5G_UE.aasx` → Complete AAS model in .aasx format  
  Includes the main shell and multiple Submodels describing device identity, technical features, network configuration, positioning, and quality of service.

## Model structure

The model consists of:
- **Common Submodels** (as specified in the IDTA guidelines):
- `Identification` – General metadata describing the digital asset
- `TechnicalData` – Basic technical attributes of the 5G UE
- `Documentation` – Attached documentation or external references (e.g., manuals, diagrams, certificates)
- `Nameplate` – Manufacturer and product identity (manufacturer, model, serial number, hardware/software revisions, year of construction, etc.)
  
- **5G-specific Submodels**:
  - `AuthenticationCertificate` — X.509 certificate for secure device authentication
  - `UE Identity` — Permanent and temporary identifiers according to 3GPP (e.g., SUPI, PEI, GUTI, MSISDN)
  - `NetworkAccessRestrictions` — Geofencing and cell-based access constraints
  - `PositioningData` — Geo-coordinates and radio signal strength/quality (RSRP, SINR, CQI, etc.)
  - `QoS` — Requested, guaranteed, and observed connection quality parameters

## How to view the model

To explore or edit the model:
1. Download AASX Package Explorer v2024-05-08
2. Launch the software and choose `File → Open`
3. Load the `5G_UE.aasx` file from this repository


---

