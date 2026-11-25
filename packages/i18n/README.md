# Regle rules I18n for Vue I18n

This is i18n translations using Vue I18n for Regle rules

## Introduction

```bash
pnpm i @regle-rules/i18n
```

## Usage

```
import { defineRegleConfig } from '@regle/core'
import { useI18n } from 'vue-i18n'

import { required } from '@regle-rules/i18n'

export const { useRegle: useRegleI18n } = defineRegleConfig({
  rules: () => {
    const i18n = useI18n()
    return {
      required: required(i18n),
    }
  },
})
```
