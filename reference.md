# Reference
## Quotes
<details><summary><code>client.quotes.<a href="/src/api/resources/quotes/client/Client.ts">showQuote</a>({ ...params }) -> YasminaaiApi.QuoteResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.quotes.showQuote({
    id: 1
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `YasminaaiApi.GetQuoteRequestsIdRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `QuotesClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.quotes.<a href="/src/api/resources/quotes/client/Client.ts">deleteQuote</a>({ ...params }) -> YasminaaiApi.DeleteQuoteRequestsIdResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.quotes.deleteQuote({
    id: 1
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `YasminaaiApi.DeleteQuoteRequestsIdRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `QuotesClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.quotes.<a href="/src/api/resources/quotes/client/Client.ts">listQuotes</a>() -> YasminaaiApi.GetQuoteRequestsResponse</code></summary>
<dl>
<dd>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.quotes.listQuotes();

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**requestOptions:** `QuotesClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.quotes.<a href="/src/api/resources/quotes/client/Client.ts">requestQuotes</a>({ ...params }) -> YasminaaiApi.QuoteResponse</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

For getting prices with benefits. 
The Quote IDs can be used later to issue a policy
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.quotes.requestQuotes({
    owner_id: "owner_id",
    phone: "phone",
    birthdate: "2023-01-15",
    car_sequence_number: "car_sequence_number",
    car_estimated_cost: 1.1
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `YasminaaiApi.PostQuoteRequestsRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `QuotesClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## Policies
<details><summary><code>client.policies.<a href="/src/api/resources/policies/client/Client.ts">showPolicy</a>({ ...params }) -> YasminaaiApi.Policy</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Show a specific policy
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.policies.showPolicy({
    carPolicy: 1
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `YasminaaiApi.GetPoliciesCarPolicyRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `PoliciesClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.policies.<a href="/src/api/resources/policies/client/Client.ts">listPolicies</a>({ ...params }) -> YasminaaiApi.Policy[]</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

Listing requested policies
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.policies.listPolicies();

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `YasminaaiApi.GetPoliciesRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `PoliciesClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.policies.<a href="/src/api/resources/policies/client/Client.ts">issuePolicy</a>({ ...params }) -> YasminaaiApi.Policy</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

For issuing a new policy
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.policies.issuePolicy({
    quote_request_id: 123,
    quote_reference_id: "550e8400-e29b-41d4-a716-446655440000",
    quote_price_id: "550e8400-e29b-41d4-a716-446655440001"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `YasminaaiApi.PostPoliciesRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `PoliciesClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

## OtPs
<details><summary><code>client.otPs.<a href="/src/api/resources/otPs/client/Client.ts">requestOtpForQuoteVerification</a>({ ...params }) -> void</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

This endpoint sends a one-time password (OTP) to the provided email and phone number for quote verification. It should be called before creating a quote request.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.otPs.requestOtpForQuoteVerification({
    email: "someone@example.com",
    phone: "0501234567",
    owner_id: "1012345678"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `YasminaaiApi.PostQuoteOtpRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `OtPsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

<details><summary><code>client.otPs.<a href="/src/api/resources/otPs/client/Client.ts">requestOtpForIssuingPolicy</a>({ ...params }) -> void</code></summary>
<dl>
<dd>

#### 📝 Description

<dl>
<dd>

<dl>
<dd>

This endpoint sends a one-time password (OTP). It should be called before issuing a policy.
</dd>
</dl>
</dd>
</dl>

#### 🔌 Usage

<dl>
<dd>

<dl>
<dd>

```typescript
await client.otPs.requestOtpForIssuingPolicy({
    email: "someone@example.com",
    phone: "0501234567",
    owner_id: "1012345678",
    quote_request_id: 123,
    quote_reference_id: "550e8400-e29b-41d4-a716-446655440000",
    quote_price_id: "550e8400-e29b-41d4-a716-446655440001"
});

```
</dd>
</dl>
</dd>
</dl>

#### ⚙️ Parameters

<dl>
<dd>

<dl>
<dd>

**request:** `YasminaaiApi.PostIssueOtpRequest` 
    
</dd>
</dl>

<dl>
<dd>

**requestOptions:** `OtPsClient.RequestOptions` 
    
</dd>
</dl>
</dd>
</dl>


</dd>
</dl>
</details>

