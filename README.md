Method-level-security:if (role.equalsIgnoreCase("admin")) {//					            	authorities.add(new SimpleGrantedAuthority("ROLE_ADMIN"));	role = "ROLE_ADMIN";	}
Collection<GrantedAuthority> authorities = AuthorityUtils.createAuthorityList(role);Authentication authentication = new UsernamePasswordAuthenticationToken(username, null,	authorities);					SecurityContextHolder.getContext().setAuthentication(authentication);SecurityContext securityContext = SecurityContextHolder.getContext();
// Authentication authentication1 = securityContext.getAuthentication();if(principal instanceof UserDetails) {//						        	UserDetails u = (UserDetails) principal ;// }
https://springbootdev.com/2017/08/30/difference-between-secured-rolesallowed-and-preauthorizepostauthorize/
https://spring.io/guides/topicals/spring-security-architecture
https://dzone.com/articles/spring-security-authentication
https://stackoverflow.com/questions/28410690/preauthorize-error-handling
https://www.baeldung.com/spring-security-create-new-custom-security-expression
https://www.petrikainulainen.net/programming/spring-framework/spring-from-the-trenches-invoking-a-secured-method-from-a-scheduled-job/
https://abhirampal.com/2016/04/15/spring-security-customising-method-level-security/

org.springframework.security.access.AccessDeniedException: Access is denied

Password Hashing, Salts, Peppers | Explained! : https://www.youtube.com/watch?v=--tnZMuoK3E   https://www.youtube.com/watch?v=f3uAsF3RaCg&list=PLqq-6Pq4lTTbEzejFKFRYfkLGYyOOwq58

aplication level security : https://www.youtube.com/watch?v=sm-8qfMWEV8&list=PLqq-6Pq4lTTYTEooakHchTGglSvkZAjnE

https://dzone.com/articles/encryption-part-2-public-key-private-key-encryptio
asymmetric encryption - Public Key Encryption or PKE 
Encrypt Password with public key in angular/react and Decrypt the password with private key in spring boot
symmetric encryption -same key use to encrypt or decrypt
