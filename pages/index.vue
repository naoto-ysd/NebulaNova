<template>
    <div class="container">
      <header class="header">
        <h1>NebulaNova</h1>
      </header>
      <main class="main">
        <h2>Welcome to NebulaNova</h2>
        <p>Innovation meets simplicity.</p>
        <a href="#" class="btn">Explore More</a>
      </main>
      <footer class="footer">
        <p>&copy; {{ year }} NebulaNova. All rights reserved.</p>
      </footer>
    </div>
  </template>

<script setup lang="ts">
  // 年を取得
  const year = new Date().getFullYear();
</script>

<style scoped>
  /* コンテナ全体を縦方向に並べる */
  .container {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
    font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
  }

  /* ヘッダー部分のスタイル */
  .header {
    background-color: #1d4ed8;
    color: #fff;
    padding: 1rem;
    text-align: center;
  }

  /* メインコンテンツのスタイル */
  .main {
    flex: 1;
    padding: 2rem;
    text-align: center;
  }

  /* ボタンのスタイル */
  .btn {
    display: inline-block;
    margin-top: 1rem;
    padding: 0.5rem 1.5rem;
    border: 2px solid #1d4ed8;
    border-radius: 4px;
    color: #1d4ed8;
    text-decoration: none;
    transition: background-color 0.3s ease, color 0.3s ease;
  }

  .btn:hover {
    background-color: #1d4ed8;
    color: #fff;
  }

  /* フッター部分のスタイル */
  .footer {
    background-color: #f5f5f5;
    padding: 1rem;
    text-align: center;
    color: #777;
  }
</style>
