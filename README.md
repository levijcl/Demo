# Demo
A simple demo for static site in spring boot

## Deploy static frontend

 ### Deploy 思路

- 使用spring boot內建的context，讓他可以直接顯示public index的檔案，
並且前端使用HashRouter，可以避開直接打spring boot API．舉例來說
`localhost:8080/` 這個會直接得到靜態網站資源，也就是前端的畫面，
但如果這時候用`localhost:8080/home`，會被spring boot吃掉，碰不到網頁，
所以用hash router可以巧妙地避開這個路徑，畢竟前端的routing跟後端的routing是完全不一樣的
