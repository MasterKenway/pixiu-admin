<!--Licensed to the Apache Software Foundation (ASF) under one or more
contributor license agreements.  See the NOTICE file distributed with
this work for additional information regarding copyright ownership.
The ASF licenses this file to You under the Apache License, Version 2.0
(the "License"); you may not use this file except in compliance with
the License.  You may obtain a copy of the License at

     http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.-->

<template>
  <div class="common">
    <div class="common-left">{{title}}</div>
    <div class="common-right">
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CommonTitle',
  props: ['title']
}
</script>

<style lang="less" scoped>
.common {
  height: 40px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-left: 12px;
  padding-right: 16px;
  background: #fff;
  box-sizing: border-box;
}
.common-left {
  display: flex;
  align-items: center;
  font-size: 18px;
  color: #303133;
  font-weight: 600;
}
.common-left::before {
  content: '';
  display: inline-block;
  width: 3px;
  height: 14px;
  background: #409EFF;
  margin-right: 5px;
}
</style>