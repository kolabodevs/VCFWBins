## bixby_error_codes

```
// Bixby Status code which is updated into the Bibxy MP0 FW_STATUS register

typedef enum BIXBY_BL_TRACE_CODE_T
{
    BIXBY_SUCCESS_BL_ENTRY                  = 0xB0,  // Bixby BL in steady state
    BIXBY_SUCCESS_AUTHENTICATION            = 0xB1,  // Bixby Authenticated successfully
    BIXBY_SUCCESS_FW_HEADER_LOAD_DONE       = 0xB2,  // Bixby FW header load done
    BIXBY_SUCCESS_FW_HEADER_VERIFIED        = 0xB3,  // Bixby FW header verified
    BIXBY_SUCCESS_FW_SIGN_LOAD_DONE         = 0xB4,  // Bixby FW Signature load done
    BIXBY_SUCCESS_FW_SIGNATURE              = 0xB5,  // Bixby FW Signaure copy done
    BIXBY_SUCCESS_FW_LOAD_DONE              = 0xB6,  // Bixby MP1 f/w downloaded successfully
    BIXBY_SUCCESS_FW_BIN_VERIFIED           = 0xB7,  // Bixby FW Binary successfully verified
    BIXBY_SUCCESS_MP1_RESET_DONE            = 0xB8,  // Bixby MP1 reset done
    BIXBY_SUCCESS_UNLOCK_DONE               = 0xB9,  // Bixby Unlock done successfully
    BIXBY_SUCCESS_PSP_SMU_MSG               = 0xBA,  // PSP SMU message sent successfully
    BIXBY_SUCCESS_USB_FW_DOWNLOAD           = 0xBB,  // USB PHY firmware downloaded successfully
} BIBXY_BL_TRACE_CODE;

typedef enum BIXBY_BL_ERROR_CODE_T
{
    BIXBY_ERR_SMN_MAP                       = 0xE0,  // Failed to map SMN
    BIXBY_ERR_CRYPTO_PASS_THRU              = 0xE1,  // Failed to Crypto Pass through
    BIXBY_AUTH_FAILED                       = 0xE2,  // Failed to authenticate Bixby
    BIXBY_ERR_LOAD_SDU_FW                   = 0xE3,  // Failed to load Bixby SDU binary
    BIXBY_ERR_FW_TYPE                       = 0xE4,  // FW type mismatch
    BIXBY_ERR_COPY_FW_SIGN                  = 0xE5,  // Failed to copy signature
    BIXBY_ERR_FW_BIN_VERIFICATION           = 0xE6,  // Binary verification failed
    BIXBY_ERR_LOAD_MP1                      = 0xE7,  // Faild to load Bixby MP1
    BIXBY_ERR_MP1_RESET                     = 0xE8,  // Failed to reset Bixby MP1
    BIXBY_ERR_USBFW_VALIDATION_FAILED       = 0xE9,  // Validation of USB PHY f/w failed
} BIBXY_BL_ERROR_CODE;
```

## bixby-fw-status-codes
```
// Bixby Status code which is updated into the Bibxy MP0 FW_STATUS register

typedef enum BIXBY_BL_TRACE_CODE_T
{
    BIXBY_SUCCESS_BL_ENTRY                  = 0xB0,  // Bixby PSP BL entry
    BIXBY_SUCCESS_ABL_LOAD_START            = 0xB1,  // Bixby ABL load started
    BIXBY_SUCCESS_ABL_LOAD_DONE             = 0xB2,  // Bixby ABL load done
    BIXBY_SUCCESS_ABL_COMPLETED_EXECUTION   = 0xB3,  // Bixby ABL completed execution
    BIXBY_SUCCESS_MP1_FW_LOAD_DONE          = 0xB4,  // Bixby MP1 f/w downloaded successfully
    BIXBY_SUCCESS_MP1_RESET_DONE            = 0xB5,  // Bixby MP1 reset done
} BIBXY_BL_TRACE_CODE;

typedef enum BIXBY_BL_ERROR_CODE_T
{
    BIXBY_ERR_SMN_MAP                       = 0xE0,  // Failed to map SMN
    BIXBY_ERR_LOAD_ABL                      = 0xE1,  // Failed to load ABL
    BIXBY_ERR_MP1_RESET                     = 0xE2,  // Failed to reset Bixby MP1
} BIBXY_BL_ERROR_CODE;
```
