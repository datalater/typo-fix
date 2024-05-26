# 제어 문자 (Control Characters)

### 1. Filter Characters에 있는 코드들을 통칭하는 개념

Filter Characters에 있는 코드들은 주로 **제어 문자 (Control Characters)** 또는 **비표시 문자 (Non-printable Characters)**로 통칭됩니다. 제어 문자는 텍스트 데이터에서 특수한 기능을 수행하거나 표시되지 않는 문자들을 포함합니다. 이러한 문자는 텍스트 영역이나 다른 사용자 인터페이스 요소에서 예기치 않은 동작을 유발할 수 있습니다.

### 2. 비슷한 성격의 유니코드 목록

다음 표는 Filter Characters와 비슷한 성격의 유니코드를 의미와 함께 정리한 것입니다:

<!-- prettier-ignore-start -->

| Unicode Character | Description                         | Encoded Value   |
|-------------------|-------------------------------------|-----------------|
| `U+0000`          | Null character                      | `%00`           |
| `U+0001`          | Start of Heading                    | `%01`           |
| `U+0002`          | Start of Text                       | `%02`           |
| `U+0003`          | End of Text                         | `%03`           |
| `U+0004`          | End of Transmission                 | `%04`           |
| `U+0005`          | Enquiry                             | `%05`           |
| `U+0006`          | Acknowledge                         | `%06`           |
| `U+0007`          | Bell                                | `%07`           |
| `U+0008`          | Backspace                           | `%08`           |
| `U+0009`          | Horizontal Tab                      | `%09`           |
| `U+000A`          | Line Feed                           | `%0A`           |
| `U+000B`          | Vertical Tab                        | `%0B`           |
| `U+000C`          | Form Feed                           | `%0C`           |
| `U+000D`          | Carriage Return                     | `%0D`           |
| `U+000E`          | Shift Out                           | `%0E`           |
| `U+000F`          | Shift In                            | `%0F`           |
| `U+0010`          | Data Link Escape                    | `%10`           |
| `U+0011`          | Device Control 1                    | `%11`           |
| `U+0012`          | Device Control 2                    | `%12`           |
| `U+0013`          | Device Control 3                    | `%13`           |
| `U+0014`          | Device Control 4                    | `%14`           |
| `U+0015`          | Negative Acknowledge                | `%15`           |
| `U+0016`          | Synchronous Idle                    | `%16`           |
| `U+0017`          | End of Transmission Block           | `%17`           |
| `U+0018`          | Cancel                              | `%18`           |
| `U+0019`          | End of Medium                       | `%19`           |
| `U+001A`          | Substitute                          | `%1A`           |
| `U+001B`          | Escape                              | `%1B`           |
| `U+001C`          | File Separator                      | `%1C`           |
| `U+001D`          | Group Separator                     | `%1D`           |
| `U+001E`          | Record Separator                    | `%1E`           |
| `U+001F`          | Unit Separator                      | `%1F`           |
| `U+007F`          | Delete                              | `%7F`           |
| `U+0085`          | Next Line (NEL)                     | `%C2%85`        |
| `U+00A0`          | No-Break Space                      | `%C2%A0`        |
| `U+2028`          | Line Separator                      | `%E2%80%A8`     |
| `U+2029`          | Paragraph Separator                 | `%E2%80%A9`     |
| `U+FEFF`          | Zero Width No-Break Space (BOM)     | `%EF%BB%BF`     |
| `U+FFFD`          | Replacement Character               | `%EF%BF%BD`     |

<!-- prettier-ignore-end -->

### 표에 대한 설명

- **Control Characters (U+0000 ~ U+001F, U+007F)**: 주로 텍스트 처리를 제어하기 위한 문자들로, 텍스트 편집기나 터미널에서 사용됩니다.
- **Whitespace and Separator Characters**:
  - `U+0085`, `U+00A0`, `U+2028`, `U+2029`: 특정 환경에서 줄바꿈이나 공백으로 처리됩니다.
  - `U+FEFF` (BOM): 파일의 인코딩을 나타내기 위해 사용됩니다.
- **Replacement Character (`U+FFFD`)**: 잘못된 또는 인식할 수 없는 문자를 나타내기 위해 사용됩니다.

이 표는 제어 문자와 비표시 문자를 포함하여, 텍스트 처리 과정에서 문제가 될 수 있는 유니코드 문자의 리스트를 제공하며, 이 문자들이 어떻게 인코딩되는지를 보여줍니다.
