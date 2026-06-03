<template>
  <div class="page-container feedback-page-container">
    <div class="help-info-item description">🏞️ {{ $t('feedback.text_1') }}</div>

    <div class="help-info-item">
      🌍 {{ $t('feedback.text_2') }} {{ $t('shortcut_key') }}：<code>{{ shortcutKey }}</code>
    </div>

    <div class="help-info-item">
      🦁 {{ $t('author') }}：
      <el-link type="primary" href="https://xpoet.cn/" target="_blank">@XPoet</el-link>
    </div>

    <div class="help-info-item">
      🌀 {{ $t('repo') }}：
      <el-link type="primary" href="https://github.com/XPoet/picx" target="_blank">
        https://github.com/XPoet/picx
      </el-link>
    </div>

    <div class="help-info-item">
      📖 {{ $t('document') }}：
      <el-link type="primary" href="https://picx-docs.xpoet.cn" target="_blank">
        https://picx-docs.xpoet.cn
      </el-link>
    </div>

    <div class="help-info-item">
      📚 {{ $t('feedback.text_3') }}：
      <el-link type="primary" href="https://blog.870507.xyz" target="_blank">
        https://blog.870507.xyz
      </el-link>
    </div>

    <div class="help-info-item img">
      <el-image style="width: 300rem" src="https://dh.073877.xyz:88/uploads/2026/6/3/a677911a2e410179959cdc821deefbf0.png" />
    </div>

    <div class="help-info-item red-text">
      <strong> ⚠️ {{ $t('feedback.text_4') }} </strong>
    </div>
  </div>
</template>

<script setup lang="ts">
import { computed } from 'vue'
import { getOSName } from '@/utils'

const shortcutKey = computed(() => (getOSName() === 'win' ? 'Ctrl + D' : 'Command + D'))
</script>

<style scoped lang="stylus">
@import "./feedback-info.styl"
</style>
