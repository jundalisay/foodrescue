{{ if ($.Get "signup" | default true) }}<strong>Sign up to be notified of new rescues!</strong>{{ end }}

{{< home-subscribe >}}

[build]
  command = "hugo"
  publish = "public"

[build.environment]
  HUGO_VERSION = "YOUR_HUGO_VERSION"
