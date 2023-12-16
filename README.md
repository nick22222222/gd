
    screen.blit(fon_img, (0,0))
    text = font.render("Welcome to game!!", True, (0, 0, 100))
    screen.blit(text, (x, y))
    text2 = font2.render("Welcome to game2!!", True, (110, 10, 100))
    screen.blit(text2, (x1, y1))
    textadsf = font.render("Welcome to game3!!", True, (110, 110, 100))
    screen.blit(textadsf, (x2, y2))

    keys = pygame.key.get_pressed()
    if keys[pygame.K_d]:
        x3 += speed
    if keys[pygame.K_w]:
        y3 -= speed
    if keys[pygame.K_s]:
        y3 += speed
    if keys[pygame.K_a]:
        x3 -= speed



    screen.blit(hero_img, (x3, y3))


    pygame.display.update()
