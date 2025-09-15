<div class="alert alert-info"><strong>Note</strong>: Datadog charges for <strong>ingested and indexed</strong> spans sent from your Android applications, but does not charge for the underlying devices. Learn more in the <a href="/account_management/billing/apm_tracing_profiler/">APM billing documentation</a>.</div>

The Datadog Tracer implements the [OpenTelemetry][1] standard, and we recommend using it as an interface for tracing your application. See [this][3] page for instructions on setting up OpenTelemetry integration with the SDK. However, the OpenTelemetry specification library **[requires desugaring][2]** to be enabled for projects with a `minSdk` < `26`. If this requirement cannot be met in your project, you can still use the Trace product with the Datadog API.

**Note**: The internal *Datadog tracing implementation* helps you transition from OpenTracing to OpenTelemetry. However, it may be removed in future releases of the SDK.

[1]: /tracing/trace_collection/custom_instrumentation/android/otel
[2]: https://github.com/open-telemetry/opentelemetry-java?tab=readme-ov-file#requirements
[3]: /tracing/trace_collection/custom_instrumentation/android/otel/?tab=kotlin

