# Dynamic Colors

```html
<style>
    .fill {
        color: #fff;
    }

    .base {
        color: #000;
    }

    .tagline {
        color: #1a1a1a;
    }

    @media (prefers-color-scheme: dark) {
        .fill {
            color: #000;
        }

        .base {
            color: #fff;
        }

        .tagline {
            color: #e8e8e8;
        }
    }
</style>
```

```diff
- <path fill="#000">
- <path fill="#fff">
- <path fill="#e8e8e8">
+ <path class="fill" fill="currentColor">
+ <path class="base" fill="currentColor">
+ <path class="tagline" fill="currentColor">
```