# OpenXR Extension Registry Audit

*Generated 2026-03-11 -- Task 3.1*

## Executive Summary

This audit examines Meta's contribution to the Khronos OpenXR extension registry and evaluates the claim that Meta authored approximately 67% of all OpenXR extensions.

## Extension Counts

| Category | Count |
|----------|-------|
| KHR (Khronos ratified) | 34 |
| EXT (Cross-vendor) | 43 |
| FB (Meta/Facebook) | 41 |
| META | 35 |
| Other vendor-specific | 112 |
| **Total** | **265** |

## Meta Contribution Analysis

- **Meta total extensions (XR_FB_ + XR_META_):** 76
- **Percentage of all extensions:** 28.7%
- **Percentage of vendor-specific extensions:** 40.4%

## 67% Claim Assessment

NOT VERIFIED against total: Meta has 28.7% of total extensions (76/265). 

## Vendor Breakdown

| Vendor Prefix | Extension Count |
|---------------|----------------|
| EXT | 43 |
| FB | 41 |
| META | 35 |
| KHR | 34 |
| BD | 21 |
| ML | 19 |
| ANDROID | 18 |
| MSFT | 15 |
| HTC | 10 |
| VARJO | 7 |
| OCULUS | 4 |
| LOGITECH | 2 |
| MNDX | 2 |
| MND | 2 |
| QCOM | 2 |
| ACME | 1 |
| ALMALENCE | 1 |
| EPIC | 1 |
| EXTX | 1 |
| HTCX | 1 |
| HUAWEI | 1 |
| OPPO | 1 |
| ULTRALEAP | 1 |
| VALVE | 1 |
| YVR | 1 |

## Meta Extensions (Full List)

- `XR_FB_android_surface_swapchain_create`
- `XR_FB_body_tracking`
- `XR_FB_color_space`
- `XR_FB_composition_layer_alpha_blend`
- `XR_FB_composition_layer_depth_test`
- `XR_FB_composition_layer_image_layout`
- `XR_FB_composition_layer_secure_content`
- `XR_FB_composition_layer_settings`
- `XR_FB_display_refresh_rate`
- `XR_FB_eye_tracking_social`
- `XR_FB_face_tracking`
- `XR_FB_face_tracking2`
- `XR_FB_foveation`
- `XR_FB_foveation_configuration`
- `XR_FB_foveation_vulkan`
- `XR_FB_hand_tracking_aim`
- `XR_FB_hand_tracking_capsules`
- `XR_FB_hand_tracking_mesh`
- `XR_FB_haptic_amplitude_envelope`
- `XR_FB_haptic_pcm`
- `XR_FB_keyboard_tracking`
- `XR_FB_passthrough`
- `XR_FB_passthrough_keyboard_hands`
- `XR_FB_render_model`
- `XR_FB_scene`
- `XR_FB_scene_capture`
- `XR_FB_space_warp`
- `XR_FB_spatial_entity`
- `XR_FB_spatial_entity_container`
- `XR_FB_spatial_entity_query`
- `XR_FB_spatial_entity_sharing`
- `XR_FB_spatial_entity_storage`
- `XR_FB_spatial_entity_storage_batch`
- `XR_FB_spatial_entity_user`
- `XR_FB_swapchain_update_state`
- `XR_FB_swapchain_update_state_android_surface`
- `XR_FB_swapchain_update_state_opengl_es`
- `XR_FB_swapchain_update_state_vulkan`
- `XR_FB_touch_controller_pro`
- `XR_FB_touch_controller_proximity`
- `XR_FB_triangle_mesh`
- `XR_META_automatic_layer_filter`
- `XR_META_body_tracking_calibration`
- `XR_META_body_tracking_calibration_`
- `XR_META_body_tracking_full_body`
- `XR_META_body_tracking_full_body_`
- `XR_META_colocation_discovery`
- `XR_META_colocation_discovery_`
- `XR_META_detached_controllers`
- `XR_META_detached_controllers_`
- `XR_META_environment_depth`
- `XR_META_foveation_eye_tracked`
- `XR_META_hand_tracking_microgestures`
- `XR_META_hand_tracking_microgestures_`
- `XR_META_headset_id`
- `XR_META_local_dimming`
- `XR_META_passthrough_color_lut`
- `XR_META_passthrough_layer_resumed_event`
- `XR_META_passthrough_layer_resumed_event_`
- `XR_META_passthrough_preferences`
- `XR_META_performance_metrics`
- `XR_META_recommended_layer_resolution`
- `XR_META_simultaneous_hands_and_controllers`
- `XR_META_simultaneous_hands_and_controllers_`
- `XR_META_spatial_entity_discovery`
- `XR_META_spatial_entity_discovery_`
- `XR_META_spatial_entity_group_sharing`
- `XR_META_spatial_entity_group_sharing_`
- `XR_META_spatial_entity_mesh`
- `XR_META_spatial_entity_persistence`
- `XR_META_spatial_entity_persistence_`
- `XR_META_spatial_entity_sharing`
- `XR_META_spatial_entity_sharing_`
- `XR_META_touch_controller_plus`
- `XR_META_virtual_keyboard`
- `XR_META_vulkan_swapchain_create_info`

## Dependency Analysis

No direct cross-vendor or third-party dependencies on Meta extensions were detected in the spec text. This may indicate that Meta extensions are primarily standalone vendor features rather than foundational building blocks.

## Strategic Implications

### Standards Capture Assessment

Meta's dominant position in the OpenXR extension registry raises several strategic considerations:

1. **Volume dominance:** Meta's extension count represents a significant share (28.7%) of the total registry, giving Meta outsized influence over the direction of the standard.

2. **Vendor lock-in risk:** Applications built against XR_FB_* and XR_META_* extensions are inherently tied to Meta's runtime. This creates a de facto platform lock-in within an ostensibly open standard.

3. **Governance leverage:** Heavy contribution to a standards body's specification can translate to governance influence, as the contributing company's engineers become the domain experts that other members defer to.

4. **Open-washing vector:** High extension counts can be cited as evidence of 'open' contribution while the extensions themselves serve to extend Meta's proprietary platform capabilities.

## Methodology

Extensions were collected from:
- Khronos registry: `https://registry.khronos.org/OpenXR/specs/1.1/man/html/`
- GitHub repository: `https://api.github.com/repos/KhronosGroup/OpenXR-Docs/contents/specification/sources/chapters/extensions`

Categorisation is based on the standard OpenXR vendor prefix convention (XR_FB_, XR_META_ for Meta; XR_KHR_, XR_EXT_ for cross-vendor; all others as third-party vendor).
