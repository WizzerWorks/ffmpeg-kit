# FFmpegKit ![GitHub release](https://img.shields.io/badge/release-v4.5-blue.svg) ![Maven Central](https://img.shields.io/maven-central/v/com.arthenica/ffmpeg-kit-min) ![CocoaPods](https://img.shields.io/cocoapods/v/ffmpeg-kit-ios-min)

FFmpeg Kit for applications.

<img src="https://github.com/tanersener/ffmpeg-kit/blob/development/docs/assets/ffmpeg-kit-icon-v9.png" width="240">

### 1. Features
- Scripts to build FFmpeg libraries
- `FFmpegKit` wrapper library to run `FFmpeg`/`FFprobe` commands in applications
- Supports Android, iOS, macOS and tvOS
- Based on FFmpeg `v4.5-dev` with optional system and external libraries
- 8 prebuilt binary packages available at [Github](https://github.com/tanersener/ffmpeg-kit/releases), [Maven Central](https://search.maven.org) and [CocoaPods](https://cocoapods.org).
- Licensed under `LGPL 3.0`, or `GPL v3.0` if GPL licensed libraries are enabled

### 2. Android

See [Android](https://github.com/tanersener/ffmpeg-kit/tree/development/android) to learn more about `FFmpegKit` for 
`Android`. 

### 3. iOS, macOS, tvOS

See [Apple](https://github.com/tanersener/ffmpeg-kit/tree/development/apple) to use `FFmpegKit` on `Apple` platforms 
(`iOS`, `macOS`, `tvOS`). 

### 4. Build Scripts

Use `android.sh`, `ios.sh`, `macos.sh` and `tvos.sh` to build `FFmpegKit` for each platform.

All scripts support additional options to enable optional libraries and disable platform architectures.

### 5. FFmpegKit Library

`FFmpegKit` is a wrapper library that allows you to easily run `FFmpeg`/`FFprobe` commands in applications. It 
provides additional features on top of `FFmpeg` to enable platform specific resources, control how commands are 
executed and how the results are handled.

`Android` library has a `Java` API and `Apple` libraries (`iOS`, `macOS`, `tvOS`) have an `Objective-C` API, 
which are identical in terms of features and capabilities.

### 6. Binary Packages

There are eight different `ffmpeg-kit` packages distributed on 
[Github](https://github.com/tanersener/ffmpeg-kit/releases), 
[Maven Central](https://search.maven.org) and [CocoaPods](https://cocoapods.org). 
Below you can see which system libraries and external libraries are enabled in each one of them. 

Please remember that some parts of `FFmpeg` are licensed under the `GPL` and only `GPL` licensed `ffmpeg-kit` packages 
include them.

<table>
<thead>
<tr>
<th align="center"></th>
<th align="center"><sup>min</sup></th>
<th align="center"><sup>min-gpl</sup></th>
<th align="center"><sup>https</sup></th>
<th align="center"><sup>https-gpl</sup></th>
<th align="center"><sup>audio</sup></th>
<th align="center"><sup>video</sup></th>
<th align="center"><sup>full</sup></th>
<th align="center"><sup>full-gpl</sup></th>
</tr>
</thead>
<tbody>
<tr>
<td align="center"><sup>external libraries</sup></td>
<td align="center">-</td>
<td align="center"><sup>vid.stab</sup><br><sup>x264</sup><br><sup>x265</sup><br><sup>xvidcore</sup></td>
<td align="center"><sup>gmp</sup><br><sup>gnutls</sup></td>
<td align="center"><sup>gmp</sup><br><sup>gnutls</sup><br><sup>vid.stab</sup><br><sup>x264</sup><br><sup>x265</sup><br><sup>xvidcore</sup></td>
<td align="center"><sup>lame</sup><br><sup>libilbc</sup><br><sup>libvorbis</sup><br><sup>opencore-amr</sup><br><sup>opus</sup><br><sup>shine</sup><br><sup>soxr</sup><br><sup>speex</sup><br><sup>twolame</sup><br><sup>vo-amrwbenc</sup></td>
<td align="center"><sup>dav1d</sup><br><sup>fontconfig</sup><br><sup>freetype</sup><br><sup>fribidi</sup><br><sup>kvazaar</sup><br><sup>libass</sup><br><sup>libiconv</sup><br><sup>libtheora</sup><br><sup>libvpx</sup><br><sup>libwebp</sup><br><sup>snappy</sup></td>
<td align="center"><sup>dav1d</sup><br><sup>fontconfig</sup><br><sup>freetype</sup><br><sup>fribidi</sup><br><sup>gmp</sup><br><sup>gnutls</sup><br><sup>kvazaar</sup><br><sup>lame</sup><br><sup>libass</sup><br><sup>libiconv</sup><br><sup>libilbc</sup><br><sup>libtheora</sup><br><sup>libvorbis</sup><br><sup>libvpx</sup><br><sup>libwebp</sup><br><sup>libxml2</sup><br><sup>opencore-amr</sup><br><sup>opus</sup><br><sup>shine</sup><br><sup>snappy</sup><br><sup>soxr</sup><br><sup>speex</sup><br><sup>twolame</sup><br><sup>vo-amrwbenc</sup></td>
<td align="center"><sup>dav1d</sup><br><sup>fontconfig</sup><br><sup>freetype</sup><br><sup>fribidi</sup><br><sup>gmp</sup><br><sup>gnutls</sup><br><sup>kvazaar</sup><br><sup>lame</sup><br><sup>libass</sup><br><sup>libiconv</sup><br><sup>libilbc</sup><br><sup>libtheora</sup><br><sup>libvorbis</sup><br><sup>libvpx</sup><br><sup>libwebp</sup><br><sup>libxml2</sup><br><sup>opencore-amr</sup><br><sup>opus</sup><br><sup>shine</sup><br><sup>snappy</sup><br><sup>soxr</sup><br><sup>speex</sup><br><sup>twolame</sup><br><sup>vid.stab</sup><br><sup>vo-amrwbenc</sup><br><sup>x264</sup><br><sup>x265</sup><br><sup>xvidcore</sup></td>
</tr>
<tr>
<td align="center"><sup>android system libraries</sup></td>
<td align="center" colspan=8><sup>zlib</sup><br><sup>MediaCodec</sup></td>
</tr>
<tr>
<td align="center"><sup>ios system libraries</sup></td>
<td align="center" colspan=8><sup>bzip2</sup><br><sup>AudioToolbox</sup><br><sup>AVFoundation</sup><br><sup>iconv</sup><br><sup>VideoToolbox</sup><br><sup>zlib</sup></td>
</tr>
<tr>
<tr>
<td align="center"><sup>macos system libraries</sup></td>
<td align="center" colspan=8><sup>bzip2</sup><br><sup>AudioToolbox</sup><br><sup>AVFoundation</sup><br><sup>Core Image</sup><br><sup>iconv</sup><br><sup>OpenCL</sup><br><sup>OpenGL</sup><br><sup>VideoToolbox</sup><br><sup>zlib</sup></td>
</tr>
<tr>
<td align="center"><sup>tvos system libraries</sup></td>
<td align="center" colspan=8><sup>bzip2</sup><br><sup>AudioToolbox</sup><br><sup>iconv</sup><br><sup>VideoToolbox</sup><br><sup>zlib</sup></td>
</tr>
</tbody>
</table>

 - `AVFoundation` is not available on `tvOS`
 - `VideoToolbox` is not available on LTS releases of `iOS` and `tvOS`

### 7. Versions

`FFmpegKit` binaries generated use the same major and minor version numbers as the upstream `FFmpeg` project. 

The exact version number of `FFmpeg` is obtained using `git describe --tags`. `dev` part in the version string 
indicates that `FFmpeg` source code is cloned from the `FFmpeg` `master` branch. 

|  FFmpegKit Version | FFmpeg Version | Release Date |
| :----: | :----: |:----: |
| [4.5](https://github.com/tanersener/ffmpeg-kit/releases/tag/v4.5) | 4.5-dev-2008 | Sep 18, 2021 |
| [4.5.LTS](https://github.com/tanersener/ffmpeg-kit/releases/tag/v4.5.LTS) | 4.5-dev-2008 | Sep 18, 2021 |
| [4.4](https://github.com/tanersener/ffmpeg-kit/releases/tag/v4.4) | 4.4-dev-3015 | Mar 03, 2021 |
| [4.4.LTS](https://github.com/tanersener/ffmpeg-kit/releases/tag/v4.4.LTS) | 4.4-dev-3015 | Mar 03, 2021 |

### 8. LTS Releases

`FFmpegKit` binaries are published in two release variants: `Main Release` and `LTS Release`. 

- Main releases include complete functionality of the library and support the latest SDK/API features.

- LTS releases are customized to support a wider range of devices. They are built using older API/SDK versions, so some features are not available on them.

This table shows the differences between two variants.

|        | Main Release | LTS Release |
| :----: | :----: | :----: |
| Android API Level | 24 | 16 | 
| Android Camera Access | Yes | - |
| Android Architectures | arm-v7a-neon<br/>arm64-v8a<br/>x86<br/>x86-64 | arm-v7a<br/>arm-v7a-neon<br/>arm64-v8a<br/>x86<br/>x86-64 |
| iOS Min SDK | 12.1 | 9.3 |
| iOS VideoToolbox | Yes | - |
| iOS AVFoundation | Yes | - |
| iOS Architectures | arm64<br/>arm64-simulator<br/>arm64-mac-catalyst<br/>x86-64<br/>x86-64-mac-catalyst | armv7<br/>arm64<br/>i386<br/>x86-64 |
| iOS Bundle Format | XCFrameworks | Frameworks |
| macOS Min SDK | 10.15 | 10.11 |
| macOS AVFoundation | Yes | - |
| macOS Architectures | arm64<br/>x86-64 | x86-64 |
| macOS Bundle Format | XCFrameworks | Frameworks |
| tvOS Min SDK | 11.0 | 9.2 |
| tvOS VideoToolbox | Yes | - |
| tvOS Architectures | arm64<br/>x86-64<br/>arm64-simulator | arm64<br/>x86-64 |
| tvOS Bundle Format | XCFrameworks | Frameworks |

### 9. Documentation

A more detailed documentation is available under [Wiki](https://github.com/tanersener/ffmpeg-kit/wiki).

### 10. Test Applications

You can see how `FFmpegKit` is used inside an application by running test applications created under 
[FFmpegKit Test](https://github.com/tanersener/ffmpeg-kit-test) project.

All applications are identical and supports command execution, video encoding, accessing https urls, encoding audio,
burning subtitles, video stabilisation, pipe operations and concurrent command execution.

### 11. License

`FFmpegKit` is licensed under the `LGPL v3.0`. However, if source code is built using the optional `--enable-gpl` flag
or prebuilt binaries with `-gpl` postfix are used, then `FFmpegKit` is subject to the `GPL v3.0` license.

### 12. Patents

It is not clearly explained in their documentation, but it is believed that `FFmpeg`, `kvazaar`, `x264` and `x265`
include algorithms which are subject to software patents. If you live in a country where software algorithms are
patentable then you'll probably need to pay royalty fees to patent holders. We are not lawyers though, so we recommend
that you seek legal advice first. See [FFmpeg Patent Mini-FAQ](https://ffmpeg.org/legal.html).

`openh264` clearly states that it uses patented algorithms. Therefore, if you build `ffmpeg-kit` with `openh264` and
distribute that library, then you are subject to pay MPEG LA licensing fees. Refer to
[OpenH264 FAQ](https://www.openh264.org/faq.html) page for the details.

### 13. Contributing

Feel free to submit issues or pull requests. 

Please note that `main` includes only the latest released source code. Changes planned for the next release are 
developed under the `development` branch. Therefore, if you want to create a pull request, please open it against
the `development`.

### 14. See Also

- [FFmpeg API Documentation](https://ffmpeg.org/doxygen/4.0/index.html)
- [FFmpeg Wiki](https://trac.ffmpeg.org/wiki/WikiStart)
- [FFmpeg External Library Licenses](https://www.ffmpeg.org/doxygen/4.0/md_LICENSE.html)
