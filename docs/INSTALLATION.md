# Installation and your first generation

For **3DKLYN Personal Beta 1.34.27 · Build 97** on Windows. Installation, restart and removal were checked in 3ds Max 2025. Other Max versions have not been verified.

## Install

1. Get `3DKLYN-personal-beta-1.34.27.mzp` from the [release page](https://github.com/3dklyn/3dklyn-plugin/releases/tag/v1.34.27).
2. [Verify the SHA-256 checksum](VERIFY.md).
3. Save your scene and open a fresh 3ds Max session.
4. Choose **Scripting → Run Script** and select the MZP.
5. Read the Personal Beta Terms and click **Install beta**. Choose whether to add the toolbar button.

The plugin opens after installation. Later, use its toolbar button or `Open-KLYN-Beta.ms` in the version's installation folder. The installation root is `%LOCALAPPDATA%/3DKLYN.PersonalBeta`. The beta does not require a 3DKLYN account or activation.

## Connect your provider

Open **API**, select your cloud provider, enter your own key and save. Saving the key does not start a generation. Access, balance, model availability and request charges are controlled by the provider.

For local generation, install ComfyUI separately and set its server URL in **API → ComfyUI**. Install the required model files and nodes for your selected workflow. Model weights and ComfyUI are not bundled; their separate licences apply.

## Generate and save

1. Choose **Image file → Choose image**, a camera viewport or a completed render.
2. Select the provider and model, describe a change and click **Generate**.
3. Inspect the result using **Before / After**, **Fit** and zoom.
4. Use **Save** to export. For video, choose a supported cloud video model, generate, inspect playback and use **Save as…**.

Returned images and video do not edit your scene. AI may change proportions, geometry and fine details in the output. Some models and advanced settings remain experimental.

## Update or remove

Updates are manual from [GitHub Releases](https://github.com/3dklyn/3dklyn-plugin/releases) or [3dklyn.com](https://3dklyn.com/). Save your work and restart Max before loading a different build. There is no automatic plugin updater in this beta.

Keep the exact original MZP. Its **Remove this beta** action removes that version's application files while keeping `UserData`. Unknown files stop removal so they can be preserved. Stable and older review builds are not migrated or overwritten by this separate beta.

## Troubleshooting

- **ComfyUI is unavailable:** start the server, wait until it is ready and check its URL.
- **A model is missing:** install the model and its required components in ComfyUI.
- **Insufficient GPU memory:** reduce the image size or choose a model that fits your hardware.
- **A request fails:** record the build, Max version, provider, model, steps and exact error. Review logs before sharing them.

Use [private support](https://3dklyn.com/messages.html) for sensitive details. Never post keys or passwords in an issue.

Source: the [official guide](https://3dklyn.com/guide.html). See the [Personal Beta Licence](https://3dklyn.com/legal/license.html) and [terms](https://3dklyn.com/legal/terms.html) for use conditions.
