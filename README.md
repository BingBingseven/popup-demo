# popup-demo
# 情景：经过ajax获取数据，再打开新页面，到第三方支付，但会被浏览器拦截（前提在于打开第三方支付页面只能用post请求）
# 解决方案：只要经过了ajax，有一定的时间延迟，浏览器都认为打开新窗口的操作不是用户手动发起，浏览器会自主屏蔽，因此产生这个解决方案。无论是何种打开新页面的方式，都有这样的问题，所以只需把打开新页面的操作提至ajax请求前面，尽可能和触发事件靠近
