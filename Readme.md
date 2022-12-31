## React Query -- @tanstack/react-query.

\_Là một thư viện hook quản lý dữ liệu requests

\_ Ý tưởng của thư viện này là để lưu trữ những gì ta fetch từ database.

\_Ví dụ: khi ta đã fetch details of pet ID 1, ta sẽ không muốn fetch lại lần nữa mà muốn lấy từ cache. Thư viện này sẽ giúp ta làm điều đó.

## Các bước thực hiện

1. Wrap our app in a query client (<QueryClientProvider><QueryClientProvider/>)
2. Instantiate a query client (give it a cache and stale times)
3. Create function request API
4. Tại nơi cần request API, import useQuery([listKeys], callback), hàm này sẽ trả cho ta một object chứa dữ liệu từ fetch và các properties thuận tiện.

## Chú ý

1. useQuery sử dụng queryClient để biết được dữ liệu đó đã fetch chưa, nếu rồi nó sẽ chỉ đơn giản lấy ra từ bộ nhớ và trả cho biến.
