# Beyond the Demo: Building RAG Systems That Actually Work -- Companion Repository

This repository contains the complete source code referenced in *Beyond the Demo: Building RAG Systems That Actually Work*.

## Code Status and Usage

### ⚠️ Important Notice

**The code in this repository is provided as reference material and educational content. It has NOT been fully tested in production environments.**

### Code Categories

#### 1. Production-Ready Patterns
These are well-established algorithms and patterns that should work as-is:
- Basic chunking strategies (fixed-size, sentence-aware)
- Standard retrieval metrics (precision@k, recall@k, MRR, NDCG)
- Vector similarity calculations
- Cost estimation formulas

**Status:** Based on industry best practices. Adapt to your specific stack.

#### 2. Illustrative/Architectural Code
These demonstrate approaches and require adaptation:
- Multi-agent RAG systems
- Autonomous research agents
- Federated RAG implementations
- Advanced retrieval patterns (query routing, fusion)

**Status:** Architectural sketches showing the approach. You'll need to:
- Add error handling
- Integrate with your infrastructure
- Implement missing helper methods
- Add proper logging and monitoring

#### 3. Simplified for Clarity
These are intentionally stripped down for readability:
- Class `__init__` methods may omit parameters
- Helper methods marked with `# Simplified` or `# Placeholder`
- Security implementations shown as pseudocode
- Async/await patterns omitted for brevity

**Status:** Conceptual examples. Do not use as-is in production.

### What's Missing

Before using any code in production, you should add:

1. **Error Handling**
   - Try/catch blocks
   - Graceful degradation
   - Retry logic with exponential backoff

2. **Production Hardening**
   - Input validation and sanitization
   - Rate limiting
   - Circuit breakers
   - Timeout handling

3. **Observability**
   - Structured logging
   - Metrics collection
   - Distributed tracing
   - Health checks

4. **Security**
   - Authentication and authorization
   - Secrets management
   - Audit logging
   - Input/output validation

5. **Testing**
   - Unit tests
   - Integration tests
   - Load tests
   - Security tests

### Using This Code

1. **Start with Chapter 14** (Conclusion) for the implementation roadmap
2. **Read the chapter first** before using any code snippet
3. **Adapt to your stack** - Examples are framework-agnostic
4. **Test thoroughly** in a non-production environment
5. **Add monitoring** before deploying to production

### Security-Critical Code

Special attention needed for:
- **RBAC middleware** (Chapter 11, Appendix A.2)
- **Tenant isolation** (Chapter 11, Appendix A.4)
- **PII detection** (Chapter 11)
- **Output moderation** (Chapter 11)

These require security review before production use.

## Key Files

### Critical Code Snippets (Appendix A)
- `A.1` Late chunking implementation
- `A.2` RBAC-enforced retrieval middleware
- `A.3` Hallucination loop detection
- `A.4` Context leakage prevention in caching
- `A.5` Autonomous research agent (full implementation)

### Architecture Diagrams (Appendix B)
- `B.1` Complete RAG pipeline flowchart
- `B.2` Multi-tenant vector database with RBAC
- `B.3` Conversational RAG state management
- `B.4` On-premise deployment architecture
- `B.5` Secure caching architecture

### Reference Tables (Appendix C)
- Retrieval metrics formulas
- Generation metrics definitions
- End-to-end evaluation criteria

## Contributing

This is a companion to the published book. For corrections or suggestions:
1. Open an issue describing the problem
2. Reference the specific chapter and line number
3. Provide the suggested correction

## License

The content of this repository is provided for educational purposes. Refer to your copy of *Beyond the Demo: Building RAG Systems That Actually Work* for usage rights.

## Disclaimer

THE CODE IN THIS REPOSITORY IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE CODE OR THE USE OR OTHER DEALINGS IN THE CODE.

The book ource code file is a password protected zip file. The password is the first word (9 characters, first character in Upcase ) under Abstract section from the book.
---

**Book:** Beyond the Demo: Building RAG Systems That Actually Work  
**Total Word Count:** ~72,000 words across 14 chapters  
**Last Updated:** February 2025
