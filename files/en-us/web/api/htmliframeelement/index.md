---
title: HTMLIFrameElement
slug: Web/API/HTMLIFrameElement
page-type: web-api-interface
browser-compat: api.HTMLIFrameElement
---

{{APIRef("HTML DOM")}}

The **`HTMLIFrameElement`** interface provides special properties and methods (beyond those of the {{domxref("HTMLElement")}} interface it also has available to it by inheritance) for manipulating the layout and presentation of inline frame elements.

{{InheritanceDiagram}}

## Instance properties

_Inherits properties from its parent, {{domxref("HTMLElement")}}_.

- {{domxref("HTMLIFrameElement.align")}} {{Deprecated_Inline}}
  - : A string that specifies the alignment of the frame with respect to the surrounding context.
- {{domxref("HTMLIFrameElement.allow")}}
  - : A string that indicates the [Permissions Policy](/en-US/docs/Web/HTTP/Guides/Permissions_Policy) specified for this `<iframe>`.
- {{domxref("HTMLIFrameElement.allowFullscreen")}}
  - : A boolean value indicating whether the inline frame is willing to be placed into full screen mode. See [Using fullscreen mode](/en-US/docs/Web/API/Fullscreen_API) for details.
- {{domxref("HTMLIFrameElement.allowPaymentRequest")}} {{Deprecated_Inline}} {{Non-standard_Inline}}
  - : A boolean value indicating whether the [Payment Request API](/en-US/docs/Web/API/Payment_Request_API) may be invoked inside a cross-origin iframe.
- {{domxref("HTMLIFrameElement.browsingTopics")}} {{Experimental_Inline}} {{non-standard_inline}}
  - : A boolean property specifying that the selected topics for the current user should be sent with the request for the associated {{htmlelement("iframe")}}'s source. This reflects the `browsingtopics` content attribute value.
- {{domxref("HTMLIFrameElement.contentDocument")}} {{ReadOnlyInline}}
  - : Returns a {{domxref("Document")}}, the active document in the inline frame's nested browsing context.
- {{domxref("HTMLIFrameElement.contentWindow")}} {{ReadOnlyInline}}
  - : Returns a {{glossary("WindowProxy")}}, the window proxy for the nested browsing context.
- {{domxref("HTMLIFrameElement.credentialless")}} {{Experimental_Inline}}
  - : A boolean value indicating whether the `<iframe>` is credentialless, meaning that its content is loaded in a new, ephemeral context. This context does not have access to the parent context's shared storage and credentials. In return, the {{httpheader("Cross-Origin-Embedder-Policy")}} (COEP) embedding rules can be lifted, so documents with COEP set can embed third-party documents that do not. See [IFrame credentialless](/en-US/docs/Web/Security/IFrame_credentialless) for a deeper explanation.
- {{domxref("HTMLIFrameElement.csp")}} {{Experimental_Inline}}
  - : Specifies the Content Security Policy that an embedded document must agree to enforce upon itself.
- {{domxref("HTMLIFrameElement.featurePolicy")}} {{ReadOnlyInline}} {{Experimental_Inline}}
  - : Returns the {{domxref("FeaturePolicy")}} interface which provides a simple API for introspecting the [Permissions Policies](/en-US/docs/Web/HTTP/Guides/Permissions_Policy) applied to a specific document.
- {{domxref("HTMLIFrameElement.frameBorder")}} {{Deprecated_Inline}}
  - : A string that indicates whether to create borders between frames.
- {{domxref("HTMLIFrameElement.height")}}
  - : A string that reflects the [`height`](/en-US/docs/Web/HTML/Reference/Elements/iframe#height) HTML attribute, indicating the height of the frame.
- {{domxref("HTMLIFrameElement.loading")}}
  - : A string providing a hint to the browser that the iframe should be loaded immediately (`eager`) or on an as-needed basis (`lazy`).
    This reflects the [`loading`](/en-US/docs/Web/HTML/Reference/Elements/iframe#loading) HTML attribute.
- {{domxref("HTMLIFrameElement.longDesc")}} {{Deprecated_Inline}}
  - : A string that contains the URI of a long description of the frame.
- {{domxref("HTMLIFrameElement.marginHeight")}} {{Deprecated_Inline}}
  - : A string being the height of the frame margin.
- {{domxref("HTMLIFrameElement.marginWidth")}} {{Deprecated_Inline}}
  - : A string being the width of the frame margin.
- {{domxref("HTMLIFrameElement.name")}}
  - : A string that reflects the [`name`](/en-US/docs/Web/HTML/Reference/Elements/iframe#name) HTML attribute, containing a name by which to refer to the frame.
- {{domxref("HTMLIFrameElement.referrerPolicy")}}
  - : A string that reflects the [`referrerPolicy`](/en-US/docs/Web/HTML/Reference/Elements/iframe#referrerpolicy) HTML attribute indicating which referrer to use when fetching the linked resource.
- {{domxref("HTMLIFrameElement.sandbox")}} {{ReadOnlyInline}}
  - : Returns a {{domxref("DOMTokenList")}} that reflects the [`sandbox`](/en-US/docs/Web/HTML/Reference/Elements/iframe#sandbox) HTML attribute, indicating extra restrictions on the behavior of the nested content.
- {{domxref("HTMLIFrameElement.scrolling")}} {{Deprecated_Inline}}
  - : A string that indicates whether the browser should provide scrollbars for the frame.
- {{domxref("HTMLIFrameElement.src")}}
  - : A string that reflects the [`src`](/en-US/docs/Web/HTML/Reference/Elements/iframe#src) HTML attribute, containing the address of the content to be embedded. Note that programmatically removing an `<iframe>`'s src attribute (e.g., via {{domxref("Element.removeAttribute()")}}) causes `about:blank` to be loaded in the frame in Firefox (from version 65), Chromium-based browsers, and Safari/iOS.
- {{domxref("HTMLIFrameElement.srcdoc")}}
  - : A string that represents the content to display in the frame.
- {{domxref("HTMLIFrameElement.width")}}
  - : A string that reflects the [`width`](/en-US/docs/Web/HTML/Reference/Elements/iframe#width) HTML attribute, indicating the width of the frame.

## Instance methods

_Also inherits methods from its parent interface, {{domxref("HTMLElement")}}._

- {{domxref("HTMLIFrameElement.getSVGDocument()")}}
  - : Returns the embedded SVG as a {{domxref("Document")}}.

## Specifications

{{Specifications}}

## Browser compatibility

{{Compat}}

## See also

- The HTML element implementing this interface: {{HTMLElement("iframe")}}
