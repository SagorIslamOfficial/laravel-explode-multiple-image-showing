# laravel-explode-multiple-image-showing

```
In your products.blade.php instead of @foreach use -
    @php $img = explode('|', $product->images); @endphp
    
And add
    <img src="/storage/image/{{$img[0]}}" style="width:100%">
```
