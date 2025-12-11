
<template>
  <div class="image-gallery">
    <h1>项目截图展示</h1>
    <p class="subtitle">以下图片展示了项目的不同页面和功能模块</p>
    
    <div class="gallery-container">
      <!-- 图片1: 注册页面 -->
      <div class="image-card">
        <div class="image-container">
          <div class="image-placeholder image-1">
            <span class="image-label">注册页面</span>
          </div>
        </div>
        <div class="image-info">
          <h3>创建账号页面</h3>
          <p>展示了用户注册流程，包含手机号输入、验证码获取和用户协议确认等功能。</p>
          <div class="image-details">
            <div class="detail-item">
              <span class="detail-label">主要功能:</span>
              <span class="detail-value">用户注册、验证码获取</span>
            </div>
            <div class="detail-item">
              <span class="detail-label">技术元素:</span>
              <span class="detail-value">表单验证、短信接口集成</span>
            </div>
            <div class="detail-item">
              <span class="detail-label">UI组件:</span>
              <span class="detail-value">输入框、按钮、复选框</span>
            </div>
          </div>
        </div>
      </div>
      
      <!-- 图片2: 扫码查看路线 -->
      <div class="image-card">
        <div class="image-container">
          <div class="image-placeholder image-2">
            <span class="image-label">扫码功能</span>
          </div>
        </div>
        <div class="image-info">
          <h3>扫码查看路线页面</h3>
          <p>提供二维码扫描功能，用户可以扫描二维码查看特定路线信息。</p>
          <div class="image-details">
            <div class="detail-item">
              <span class="detail-label">主要功能:</span>
              <span class="detail-value">二维码扫描、路线查看</span>
            </div>
            <div class="detail-item">
              <span class="detail-label">技术元素:</span>
              <span class="detail-value">摄像头API、二维码解析</span>
            </div>
            <div class="detail-item">
              <span class="detail-label">UI组件:</span>
              <span class="detail-value">扫码框、提示文字</span>
            </div>
          </div>
        </div>
      </div>
      
      <!-- 图片3: 发布功能 -->
      <div class="image-card">
        <div class="image-container">
          <div class="image-placeholder image-3">
            <span class="image-label">发布功能</span>
          </div>
        </div>
        <div class="image-info">
          <h3>发布页面</h3>
          <p>用户发布内容或信息的界面，可能包含内容输入、媒体上传和发布确认等功能。</p>
          <div class="image-details">
            <div class="detail-item">
              <span class="detail-label">主要功能:</span>
              <span class="detail-value">内容发布、信息提交</span>
            </div>
            <div class="detail-item">
              <span class="detail-label">技术元素:</span>
              <span class="detail-value">富文本编辑器、文件上传</span>
            </div>
            <div class="detail-item">
              <span class="detail-label">UI组件:</span>
              <span class="detail-value">发布按钮、表单字段</span>
            </div>
          </div>
        </div>
      </div>
      
      <!-- 图片4: 路线详情 -->
      <div class="image-card">
        <div class="image-container">
          <div class="image-placeholder image-4">
            <span class="image-label">路线详情</span>
          </div>
        </div>
        <div class="image-info">
          <h3>路线详情与导航页面</h3>
          <p>展示路线详情、预计时间和导航功能，用户可查看具体路线信息并开始导航。</p>
          <div class="image-details">
            <div class="detail-item">
              <span class="detail-label">主要功能:</span>
              <span class="detail-value">路线规划、导航、时间预估</span>
            </div>
            <div class="detail-item">
              <span class="detail-label">技术元素:</span>
              <span class="detail-value">地图API、路径规划算法</span>
            </div>
            <div class="detail-item">
              <span class="detail-label">UI组件:</span>
              <span class="detail-value">地图展示、信息面板、导航按钮</span>
            </div>
            <div class="detail-item">
              <span class="detail-label">数据示例:</span>
              <span class="detail-value">ADC80F.0I, BUC00, 26.60, 预计/10/00</span>
            </div>
          </div>
        </div>
      </div>
    </div>
    
    <div class="project-summary">
      <h2>项目总结</h2>
      <p>该项目是一个多功能的在线平台，包含用户注册、扫码查看、内容发布和路线导航等核心功能。</p>
      <p>从UI界面可以看出，项目采用了简洁现代的设计风格，注重用户体验和功能性。</p>
      <div class="tech-tags">
        <span class="tech-tag">Vue 3</span>
        <span class="tech-tag">TypeScript</span>
        <span class="tech-tag">移动端适配</span>
        <span class="tech-tag">表单处理</span>
        <span class="tech-tag">地图集成</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
// 这里可以定义组件逻辑
// 例如，如果实际应用中需要加载真实图片，可以这样定义：
interface ImageItem {
  id: number;
  title: string;
  description: string;
  url?: string; // 实际图片URL
  placeholderClass: string;
}

// 示例数据
const imageList: ImageItem[] = [
  {
    id: 1,
    title: "创建账号页面",
    description: "展示了用户注册流程，包含手机号输入、验证码获取和用户协议确认等功能。",
    placeholderClass: "image-1"
  },
  {
    id: 2,
    title: "扫码查看路线页面",
    description: "提供二维码扫描功能，用户可以扫描二维码查看特定路线信息。",
    placeholderClass: "image-2"
  },
  {
    id: 3,
    title: "发布页面",
    description: "用户发布内容或信息的界面，可能包含内容输入、媒体上传和发布确认等功能。",
    placeholderClass: "image-3"
  },
  {
    id: 4,
    title: "路线详情与导航页面",
    description: "展示路线详情、预计时间和导航功能，用户可查看具体路线信息并开始导航。",
    placeholderClass: "image-4"
  }
];

// 实际项目中，可以在这里添加图片加载、点击事件等逻辑
</script>

<style scoped>
.image-gallery {
  max-width: 1200px;
  margin: 0 auto;
  padding: 24px;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  color: #333;
}

h1 {
  text-align: center;
  color: #2c3e50;
  margin-bottom: 8px;
}

.subtitle {
  text-align: center;
  color: #7f8c8d;
  margin-bottom: 32px;
}

.gallery-container {
  display: grid;
  grid-template-columns: 1fr;
  gap: 32px;
}

@media (min-width: 768px) {
  .gallery-container {
    grid-template-columns: repeat(2, 1fr);
  }
}

.image-card {
  background-color: #fff;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
  overflow: hidden;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.image-card:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15);
}

.image-container {
  height: 200px;
  position: relative;
  overflow: hidden;
}

.image-placeholder {
  height: 100%;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  font-weight: bold;
  font-size: 1.2rem;
  position: relative;
}

.image-label {
  position: absolute;
  top: 16px;
  left: 16px;
  background-color: rgba(0, 0, 0, 0.7);
  padding: 4px 12px;
  border-radius: 20px;
  font-size: 0.9rem;
}

/* 为每个图片占位符设置不同的颜色，模拟不同图片 */
.image-1 {
  background: linear-gradient(135deg, #3498db, #8e44ad);
}

.image-2 {
  background: linear-gradient(135deg, #2ecc71, #3498db);
}

.image-3 {
  background: linear-gradient(135deg, #e74c3c, #f39c12);
}

.image-4 {
  background: linear-gradient(135deg, #1abc9c, #34495e);
}

.image-info {
  padding: 20px;
}

.image-info h3 {
  margin-top: 0;
  margin-bottom: 12px;
  color: #2c3e50;
  font-size: 1.3rem;
}

.image-info p {
  color: #555;
  line-height: 1.5;
  margin-bottom: 16px;
}

.image-details {
  background-color: #f8f9fa;
  padding: 16px;
  border-radius: 8px;
  border-left: 4px solid #3498db;
}

.detail-item {
  margin-bottom: 8px;
  display: flex;
}

.detail-item:last-child {
  margin-bottom: 0;
}

.detail-label {
  font-weight: 600;
  color: #2c3e50;
  min-width: 100px;
}

.detail-value {
  color: #555;
  flex: 1;
}

.project-summary {
  margin-top: 48px;
  padding: 24px;
  background-color: #f8f9fa;
  border-radius: 12px;
  border-top: 4px solid #2ecc71;
}

.project-summary h2 {
  color: #2c3e50;
  margin-top: 0;
}

.tech-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  margin-top: 16px;
}

.tech-tag {
  background-color: #3498db;
  color: white;
  padding: 6px 12px;
  border-radius: 20px;
  font-size: 0.85rem;
  font-weight: 500;
}
</style>
